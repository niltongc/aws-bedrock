## list models

```sh
aws bedrock list-foundation-models \
  --region us-west-2 \
  --query "modelSummaries[?contains(modelId, 'anthropic')].modelId" \
  --output text
```

```sh
aws bedrock list-inference-profiles \
  --region us-west-2 \
  --query "inferenceProfileSummaries[?status=='ACTIVE'].inferenceProfileId"
```