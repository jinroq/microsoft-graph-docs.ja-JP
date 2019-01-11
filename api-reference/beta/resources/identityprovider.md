---
title: identityProvider リソースの種類
description: Azure Active Directory (AD の Azure) id プロバイダーを表します。 Id プロバイダーは、マイクロソフト、Google、Facebook、Amazon、または LinkedIn にできます。
localization_priority: Normal
ms.openlocfilehash: 0a465b1c7b4ad7f74e6357e77da3692d64294e7e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858542"
---
# <a name="identityprovider-resource-type"></a>identityProvider リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory (AD の Azure) id プロバイダーを表します。 Id プロバイダーは、マイクロソフト、Google、Facebook、Amazon、または LinkedIn にできます。

Azure AD B2C テナント id プロバイダーを構成するを有効にします。

* ユーザーがサインアップして、コンシューマー アプリケーションでソーシャル アカウントでサインインします。 などのアプリケーションでは、Facebook のアカウントを使用してサービスにサインアップできるようにするのには Azure AD B2C を使用することができます。
* 既存のローカルのリンクは、コンシューマー アプリケーションでのソーシャル アカウントにアカウントします。 たとえば、ユーザーがユーザー名とパスワード (ローカル アカウント) のアプリケーションで作成します。 Facebook を使用してサインインできるように、Facebook アカウントに既存のローカル アカウントをリンクするのには、ユーザーが後で決定します。

B2B ゲストの将来のシナリオを有効に、Azure AD テナントの id プロバイダーを構成します。 たとえば、組織では、Gmail のユーザーと共有する必要のある Office 365 のリソースがあります。 Gmail ユーザーは認証し、ドキュメントにアクセスする Google アカウントの資格情報を使用します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[IdentityProvider を取得します。](../api/identityprovider-get.md) |identityProvider|既存の identityProvider のプロパティを読み取る。|
|[IdentityProvider を作成します。](../api/identityprovider-post-identityproviders.md)|identityProvider|新しい identityProvider を作成します。|
|[IdentityProvider を更新します。](../api/identityprovider-update.md)|なし|既存の identityProvider を更新します。|
|[IdentityProvider を削除します。](../api/identityprovider-delete.md)|なし|既存の identityProvider を削除します。|
|[リスト identityProviders](../api/identityprovider-list.md)|identityProvider コレクション|テナントで構成されているすべての identityProviders を一覧表示します。|

## <a name="properties"></a>プロパティ

|プロパティ|種類|必須|Nullable|説明|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|String|はい|いいえ|アプリケーションのクライアント ID。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。|
|clientSecret|String|はい|いいえ|アプリケーションのクライアントの機密情報です。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。 これは、書き込み専用です。 読み取り操作が返されます"\*\*\*\*」です。|
|id|String|いいえ|いいえ|Id プロバイダーの ID。|
|名前|String|いいえ|いいえ|Id プロバイダーの表示名。|
|type|String|はい|いいえ|Id プロバイダーの種類。 次の値のいずれかを指定する必要があります。 <ul><li/>Microsoft<li/>Google<li/>アマゾン<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>ID とシークレットは、クライアントを取得する場所

各 id プロバイダーには、アプリケーションの登録を作成するためのプロセスです。 など、ユーザーは、 [developers.facebook.com](https://developers.facebook.com/)で facebook アプリ登録を作成します。 結果のクライアント ID とクライアント シークレットは、 [identityProvider を作成](../api/identityprovider-post-identityproviders.md)するのに渡すことができます。 次に、ディレクトリ内の各ユーザー オブジェクトは、認証のためのテナントの id プロバイダーのいずれかに統合することができます。 Id プロバイダーのサインイン ページで資格情報を入力してサインインするのにはこれを使用できます。 テナントがアプリケーションにトークンを発行する前に、Azure AD では、id プロバイダーからトークンが検証されます。

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
