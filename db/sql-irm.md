# Immutable Relational Mapper

A simple relational database mapper for immutable objects.

## Concepts

- Less to learn.
- Less conventions: to avoid changing original code to conform to this library.
- Declarative and elegant representation: fluent, immutable, and `null`-eliminated.
- Simple features.
- Users can customize its various behaviors and it adapts to respective situations.

## Features

- **イミュータブル**の名称と**テーブル**の名称の関連づけ。
- （イミュータブルの）フィールドの型と（テーブルの）列の型の関連づけ。
- レコードからインスタンスへの自動的な変換。
- シンプルなクエリやコマンドの、SQLなしでの提供。
- SQL文 をリソースから自動的に取得する。

これらの機能を実際にどのように実現するのかは、ユーザーが指定できる。
