# google-chat-notification

A GitHub Action to send deployment notifications to Google Chat.

## Usage

```yml
- name: Google Chat Notification
  uses: DeepwalkInternal/google-chat-notification@v1
  if: always()
  with:
    webhook_url: ${{ secrets.GOOGLE_CHAT_WEBHOOK }}
    status: ${{ job.status }}
```

## Versioning

- `v1` always points to the latest `v1.x.y` release. It moves when a backward-compatible change ships, so `@v1` picks up fixes with no change to your workflow.
- Exact tags such as `v1.0.1` never move. Pin one of them, or a commit SHA, if you need the action's code to never change.
- A breaking change, such as a new required input, ships as `v2`. `v1` does not move to it.
