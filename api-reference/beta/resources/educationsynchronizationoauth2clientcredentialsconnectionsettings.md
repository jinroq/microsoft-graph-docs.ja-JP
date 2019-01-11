---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアントの資格情報の付与は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
ms.openlocfilehash: 49a0a267ddb3a8f3a954888679806ea7913e24f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822583"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="6c9cc-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="6c9cc-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="6c9cc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c9cc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c9cc-106">[OAuth2 クライアントの資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="6c9cc-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6c9cc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c9cc-108">Properties</span></span>

| <span data-ttu-id="6c9cc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c9cc-109">Property</span></span> | <span data-ttu-id="6c9cc-110">種類</span><span class="sxs-lookup"><span data-stu-id="6c9cc-110">Type</span></span> | <span data-ttu-id="6c9cc-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c9cc-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6c9cc-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="6c9cc-112">**tokenUrl**</span></span> | <span data-ttu-id="6c9cc-113">String</span><span class="sxs-lookup"><span data-stu-id="6c9cc-113">String</span></span> | <span data-ttu-id="6c9cc-114">データ プロバイダーのアクセス トークンを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="6c9cc-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="6c9cc-115">**scope**</span></span> | <span data-ttu-id="6c9cc-116">String</span><span class="sxs-lookup"><span data-stu-id="6c9cc-116">String</span></span> | <span data-ttu-id="6c9cc-117">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)です。</span><span class="sxs-lookup"><span data-stu-id="6c9cc-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c9cc-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c9cc-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
