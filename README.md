# LearnTelethon
Learn Telethon easily through this repo.

 ⭐️ Thanks **everyone** who has starred the project, it means a lot!

|logo| **Telethon** is an asyncio_ **Python 3**
MTProto_ library to interact with Telegram_'s API
as a user or through a bot account (bot API alternative).

.. important::

    If you have code using Telethon before its 1.0 version, you must
    read `Compatibility and Convenience`_ to learn how to migrate.

What is this?
-------------

Telegram is a popular messaging application. This library is meant
to make it easy for you to write Python programs that can interact
with Telegram. Think of it as a wrapper that has already done the
heavy job for you, so you can focus on developing an application.


Installing
----------

.. code-block:: sh

  pip3 install telethon


Creating a client
-----------------

.. code-block:: python

    from telethon import TelegramClient, events, sync

    # These example values won't work. You must get your own api_id and
    # api_hash from https://my.telegram.org, under API Development.
    api_id = 12345
    api_hash = '0123456789abcdef0123456789abcdef'

    client = TelegramClient('session_name', api_id, api_hash)
    client.start()

