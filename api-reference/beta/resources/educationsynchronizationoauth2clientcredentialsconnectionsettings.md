---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアントの資格情報の付与は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523555"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="7b5ed-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="7b5ed-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b5ed-104">[OAuth2 クライアントの資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="7b5ed-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="7b5ed-105">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="7b5ed-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7b5ed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b5ed-106">Properties</span></span>

| <span data-ttu-id="7b5ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b5ed-107">Property</span></span> | <span data-ttu-id="7b5ed-108">型</span><span class="sxs-lookup"><span data-stu-id="7b5ed-108">Type</span></span> | <span data-ttu-id="7b5ed-109">説明</span><span class="sxs-lookup"><span data-stu-id="7b5ed-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7b5ed-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="7b5ed-110">**tokenUrl**</span></span> | <span data-ttu-id="7b5ed-111">String</span><span class="sxs-lookup"><span data-stu-id="7b5ed-111">String</span></span> | <span data-ttu-id="7b5ed-112">データ プロバイダーのアクセス トークンを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="7b5ed-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="7b5ed-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="7b5ed-113">**scope**</span></span> | <span data-ttu-id="7b5ed-114">String</span><span class="sxs-lookup"><span data-stu-id="7b5ed-114">String</span></span> | <span data-ttu-id="7b5ed-115">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)です。</span><span class="sxs-lookup"><span data-stu-id="7b5ed-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b5ed-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b5ed-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
