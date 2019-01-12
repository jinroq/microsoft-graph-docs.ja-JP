---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアントの資格情報の付与は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8976c3a3a6088abd88cf70182040d4b3a6cc3f7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912891"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="4af7a-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="4af7a-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="4af7a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4af7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4af7a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4af7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4af7a-106">[OAuth2 クライアントの資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="4af7a-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="4af7a-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="4af7a-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4af7a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4af7a-108">Properties</span></span>

| <span data-ttu-id="4af7a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4af7a-109">Property</span></span> | <span data-ttu-id="4af7a-110">型</span><span class="sxs-lookup"><span data-stu-id="4af7a-110">Type</span></span> | <span data-ttu-id="4af7a-111">説明</span><span class="sxs-lookup"><span data-stu-id="4af7a-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4af7a-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="4af7a-112">**tokenUrl**</span></span> | <span data-ttu-id="4af7a-113">String</span><span class="sxs-lookup"><span data-stu-id="4af7a-113">String</span></span> | <span data-ttu-id="4af7a-114">データ プロバイダーのアクセス トークンを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="4af7a-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="4af7a-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="4af7a-115">**scope**</span></span> | <span data-ttu-id="4af7a-116">String</span><span class="sxs-lookup"><span data-stu-id="4af7a-116">String</span></span> | <span data-ttu-id="4af7a-117">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)です。</span><span class="sxs-lookup"><span data-stu-id="4af7a-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4af7a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4af7a-118">JSON representation</span></span>
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
