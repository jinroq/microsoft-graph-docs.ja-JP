---
title: 'educationSynchronizationProfile: uploadUrl'
description: テナントで特定の学校のデータの同期プロファイルの Azure blob ストレージにソース ファイルをアップロードする共有アクセス署名 (SAS) を取得します。 SAS トークンには、1 時間の有効期限が。
author: mmast-msft
ms.openlocfilehash: 15a4536e21307067ac55783edd9eac675ae4144b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341063"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>educationSynchronizationProfile: uploadUrl

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の Azure blob ストレージにソース ファイルをアップロードするには、共有アクセス署名 (SAS) を取得します。 SAS トークンには、1 時間の有効期限が。

アップロードのみの[CSV データ プロバイダー](../resources/educationcsvdataprovider.md)の URL が用意されています。

> **注:** SAS のトークンを使用して blob ストレージにアクセスするには、 [Azure ストレージの Sdk](https://github.com/search?q=org%3AAzure+azure-storage)または[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)を使用します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 |
|:-----------|:----------|
| 委任 (職場または学校のアカウント) | EduAdministration.ReadWrite |
|(個人用の Microsoft アカウントを委任します。|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)の SA の URL です。

かどうかは前の要求が処理中、このメソッドが返されます、 `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)のアップロードが現在ブロックされていることを示します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
