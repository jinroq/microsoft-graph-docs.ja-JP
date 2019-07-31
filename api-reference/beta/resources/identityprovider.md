---
title: identityProvider リソース タイプ
description: Azure Active Directory (Azure AD) の ID プロバイダーを表します。 Id プロバイダーは、Microsoft、Google、Facebook、Amazon、または LinkedIn にすることができます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 470d29844470df6f5cd81ba0d40156492c1fd635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971810"
---
# <a name="identityprovider-resource-type"></a>identityProvider リソース タイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) の ID プロバイダーを表します。 Id プロバイダーは、Microsoft、Google、Facebook、Amazon、または LinkedIn にすることができます。

Azure AD B2C テナントで id プロバイダーを構成すると、次のことが可能になります。

* ユーザーがサインアップして、コンシューマーアプリケーションでソーシャルアカウントを使用してサインインする。 たとえば、アプリケーションで Azure AD B2C を使用することにより、ユーザーが Facebook アカウントを使用してサービスにサインアップすることを可能にできます。
* ユーザーが既存のローカルアカウントをコンシューマーアプリケーションのソーシャルアカウントにリンクする。 たとえば、ユーザーがアプリケーションでユーザー名とパスワード (ローカル アカウント) を作成したとします。 ユーザーは後から既存のローカル アカウントを自分の Facebook アカウントに関連付けることができ、Facebook を使用してサインインできるようになります。

Azure AD テナントで ID プロバイダーを構成すると、今後の B2B ゲスト シナリオを有効にすることができます。 たとえば、Gmail のユーザーと共有する必要がある Office 365 のリソースが組織にあるとします。 Gmail ユーザーは、認証したりドキュメントにアクセスしたりするのに Google アカウントの資格情報を使用できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[identityProviderを入手する](../api/identityprovider-get.md) |identityProvider|既存の identityProvider のプロパティのプロパティを確認します。|
|[identityProvider を作成する](../api/identityprovider-post-identityproviders.md)|identityProvider|新しい identityProvider を作成します。|
|[identityProvider を更新する](../api/identityprovider-update.md)|なし|既存の identityProvider を更新します。|
|[identityProvider を削除する](../api/identityprovider-delete.md)|なし|既存の identityProvider を削除します。|
|[identityProvider を一覧表示する](../api/identityprovider-list.md)|identityProvider コレクション|テナント内で構成されているすべての identityProvider を一覧表示します。|

## <a name="properties"></a>プロパティ

|プロパティ|型|必須|Nullable|説明|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|文字列|はい|なし|アプリケーションのクライアント ID。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。|
|clientSecret|文字列|はい|なし|アプリケーションでのクライアント シークレット。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。 これは、書き込み専用です。 読み取り操作を行うと、"\*\*\*\*" が返されます。|
|id|String|いいえ|いいえ|ID プロバイダーの ID。|
|name|String|いいえ|いいえ|ID プロバイダーの表示名。|
|type|String|はい|いいえ|ID プロバイダーの型。 次のいずれかの値であることが必要です。 <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>クライアント ID とシークレットを取得する場所

各 ID プロバイダーには、アプリ登録を作成するためのプロセスがあります。 たとえば、ユーザーは Facebook とのアプリ登録を [developers.facebook.com](https://developers.facebook.com/) で作成します。 作成したクライアント ID とクライアント シークレットは、[identityProvider を作成する](../api/identityprovider-post-identityproviders.md) に渡すことができます。 その後、認証のためにディレクトリ内の各ユーザー オブジェクトをいずれかのテナントの ID プロバイダーにフェデレーションすることができます。 これにより、ID プロバイダーのサインイン ページでユーザーが資格情報を入力してサインインできるようになります。 ID プロバイダーからのトークンは、テナントがトークンをアプリケーションに発行する前に、Azure AD によって検証されます。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
