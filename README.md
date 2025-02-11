# google-chat-notification

A GitHub Action to send deployment notifications to Google Chat.

## Usage

```yml
- name: Google Chat Notification
  uses: DeepwalkInternal/google-chat-notification
  if: always()
  with:
    webhook_url: ${{ secrets.GOOGLE_CHAT_WEBHOOK }}
    status: ${{ job.status }}
```
