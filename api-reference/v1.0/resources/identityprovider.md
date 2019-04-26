---
title: identityProvider リソース タイプ
description: Azure Active Directory (Azure AD) の ID プロバイダーを表します。
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f251853704edd644f615ab986cc3188608fbbe05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567558"
---
# <a name="identityprovider-resource-type"></a>identityProvider リソース タイプ

Azure Active Directory (Azure AD) の ID プロバイダーを表します。 ID プロバイダーとして、Microsoft、Google、Facebook、Amazon、LinkedIn、または Twitter を使用できます。 次の ID プロバイダーはプレビュー段階です: Weibo、QQ、WeChat、GitHub および OpenID Connect をサポートするすべてのプロバイダー。 

Azure AD B2C テナントで ID プロバイダーを構成すると、ユーザーは次のことができるようになります。

* ソーシャル アカウントを使用しての、コンシューマー向けアプリケーションでの新規登録およびサインイン。 たとえば、アプリケーションで Azure AD B2C を使用することにより、ユーザーが Facebook アカウントを使用してサービスにサインアップすることを可能にできます。
* コンシューマー向けアプリケーションでの、既存のローカル アカウントのソーシャル アカウントへの関連付け。 たとえば、ユーザーがアプリケーションでユーザー名とパスワード (ローカル アカウント) を作成したとします。 ユーザーは後から既存のローカル アカウントを自分の Facebook アカウントに関連付けることができ、Facebook を使用してサインインできるようになります。

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
|clientId|String|はい|いいえ|アプリケーションのクライアント ID。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。|
|clientSecret|String|はい|いいえ|アプリケーションでのクライアント シークレット。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。 これは、書き込み専用です。 読み取り操作を行うと、"\*\*\*\*" が返されます。|
|id|String|いいえ|いいえ|ID プロバイダーの ID。|
|name|String|いいえ|いいえ|ID プロバイダーの表示名。|
|type|String|はい|いいえ|ID プロバイダーの型。 B2C シナリオでは、この型は次の値である必要があります。 <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat</ul>B2B シナリオでは、値は Google である必要があります。|

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
