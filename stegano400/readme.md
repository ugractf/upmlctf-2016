# Beautiful sound

> Флаги всегда звучат красиво.... или нет?
>
> [Attachment](sound.wav)

## Write-up

Если посмотреть на свойства файла, то можно обратить внимание, что это стереозвук. Однако, на обоих каналах звук почти одинаковый.
Присмотримся к спектрограмме поближе и заметим, что на одном канале чистая синусоида, а на другом — она же, но с небольшими отклонениями.
Посмотрим на числовые значения амплитуды каждого кадра дорожки. Их разницы находятся в интервале [0..255]. Попробуем перевести эти разницы в бинарный файл.
Встроенная в Linux утилита `file` подсказывает, что файл имеет расширение `png`. В нём и находился флаг.

Флаг: `png_on_uctf`
