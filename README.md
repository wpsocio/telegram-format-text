# WPSocio\TelegramFormatText

HTML to Text converter/formatter for [Telegram Bot API](https://core.telegram.org/bots/api#formatting-options)

Inspired by [thephpleague/html-to-markdown](https://github.com/thephpleague/html-to-markdown).

## Usage

```bash
composer require wpsocio/telegram-format-text
```

```php
require_once __DIR__ . '/autoload.php';

$html = 'Some html here';

$options = [
	'format_to' => 'Markdown',
];
$converter = new \WPSocio\TelegramFormatText\HtmlConverter( $options );

// The text is now safe to be sent to Telegram
$text = $converter->convert( $html );
```

## Requirements

- `PHP >= 8.0`
