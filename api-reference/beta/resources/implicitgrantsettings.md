---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。
localization_priority: Normal
ms.openlocfilehash: 82051c3605d9815fef8a0852e0ffa9075f4a6d78
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574517"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="e3bae-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3bae-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3bae-106">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3bae-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="e3bae-107">暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="e3bae-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="e3bae-108">暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3bae-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="e3bae-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3bae-109">Properties</span></span>

| <span data-ttu-id="e3bae-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3bae-110">Property</span></span> | <span data-ttu-id="e3bae-111">型</span><span class="sxs-lookup"><span data-stu-id="e3bae-111">Type</span></span> | <span data-ttu-id="e3bae-112">説明</span><span class="sxs-lookup"><span data-stu-id="e3bae-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="e3bae-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="e3bae-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="e3bae-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3bae-114">Boolean</span></span> | <span data-ttu-id="e3bae-115">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3bae-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="e3bae-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="e3bae-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="e3bae-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3bae-117">Boolean</span></span> | <span data-ttu-id="e3bae-118">この web アプリケーションで、OAuth 2.0 の暗黙的なフローを使用してアクセス トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3bae-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3bae-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3bae-119">JSON representation</span></span>
<span data-ttu-id="e3bae-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3bae-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
