## Official Senders

We have created some custom senders for typical use-cases, these senders are official supported by us and come with the same flexibility like the core-package itself.

If you want any other sender or want to provide written code for one please [create an issue](https://github.com/fenos/Notifynder/issues/new?milestone=Senders) in the core-package. If you have any questions or feature-wishes for an existing one you can create an issue in the sender-repo.

### E-Mail Sender

[Repository](https://github.com/Astrotomic/notifynder-sender-email)

With this one you can send notifications as text message via E-Mail.

```php
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendEmail();
```

### Slack Sender

[Repository](https://github.com/Astrotomic/notifynder-sender-slack) | [Slack](https://slack.com/developers)

With this one you can send notifications as text message via Slack.

```php
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendSlack();
```

### MessageBird Sender

[Repository](https://github.com/Astrotomic/notifynder-sender-messagebird) | [MessageBird](https://developers.messagebird.com)

With this one you can send notifications as SMS or Voice message via MessageBird.

```php
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendMessageBirdSms();
           
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendMessageBirdCall();
```

### Redis Sender

[Repository](https://github.com/Astrotomic/notifynder-sender-redis) | [Redis PubSub](https://laravel.com/docs/5.1/redis#pubsub)

With this one you can send notifications as json array message via redis as live messages.

```php
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendRedis();
```

### Twilio Sender

[Repository](https://github.com/Astrotomic/notifynder-sender-twilio) | [Twilio](https://www.twilio.com/docs/)

With this one you can send notifications as SMS message via Twilio.

```php
Notifynder::category('sayhello')
           ->from(1)
           ->to(2)
           ->sendTwilio();
```