---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506223"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="3cb6b-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3cb6b-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb6b-106">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="3cb6b-107">個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="3cb6b-108">暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="3cb6b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cb6b-109">Properties</span></span>

| <span data-ttu-id="3cb6b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cb6b-110">Property</span></span> | <span data-ttu-id="3cb6b-111">型</span><span class="sxs-lookup"><span data-stu-id="3cb6b-111">Type</span></span> | <span data-ttu-id="3cb6b-112">説明</span><span class="sxs-lookup"><span data-stu-id="3cb6b-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="3cb6b-113">enableidtokenissuance</span><span class="sxs-lookup"><span data-stu-id="3cb6b-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="3cb6b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cb6b-114">Boolean</span></span> | <span data-ttu-id="3cb6b-115">この web アプリケーションが OAuth 2.0 暗黙的フローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="3cb6b-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="3cb6b-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="3cb6b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cb6b-117">Boolean</span></span> | <span data-ttu-id="3cb6b-118">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してアクセストークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb6b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3cb6b-119">JSON representation</span></span>
<span data-ttu-id="3cb6b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3cb6b-120">Here is a JSON representation of the resource.</span></span>

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
