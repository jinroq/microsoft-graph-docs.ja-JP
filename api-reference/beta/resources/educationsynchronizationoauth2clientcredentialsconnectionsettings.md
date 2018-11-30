---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアントの資格情報の付与は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
ms.openlocfilehash: 901fabb802d4ed5fa0c99538e52b9a07199eb298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072207"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="829e6-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="829e6-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="829e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="829e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="829e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="829e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="829e6-106">[OAuth2 クライアントの資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="829e6-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="829e6-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="829e6-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="829e6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="829e6-108">Properties</span></span>

| <span data-ttu-id="829e6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="829e6-109">Property</span></span> | <span data-ttu-id="829e6-110">型</span><span class="sxs-lookup"><span data-stu-id="829e6-110">Type</span></span> | <span data-ttu-id="829e6-111">説明</span><span class="sxs-lookup"><span data-stu-id="829e6-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="829e6-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="829e6-112">**tokenUrl**</span></span> | <span data-ttu-id="829e6-113">String</span><span class="sxs-lookup"><span data-stu-id="829e6-113">String</span></span> | <span data-ttu-id="829e6-114">データ プロバイダーのアクセス トークンを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="829e6-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="829e6-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="829e6-115">**scope**</span></span> | <span data-ttu-id="829e6-116">String</span><span class="sxs-lookup"><span data-stu-id="829e6-116">String</span></span> | <span data-ttu-id="829e6-117">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)です。</span><span class="sxs-lookup"><span data-stu-id="829e6-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="829e6-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="829e6-118">JSON representation</span></span>
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
