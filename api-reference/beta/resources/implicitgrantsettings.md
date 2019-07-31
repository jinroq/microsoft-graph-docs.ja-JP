---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92ba18488cc2700b565be47bac3874b6d75e1c13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005794"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="3d50c-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d50c-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d50c-106">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d50c-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="3d50c-107">個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。</span><span class="sxs-lookup"><span data-stu-id="3d50c-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="3d50c-108">暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d50c-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="3d50c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d50c-109">Properties</span></span>

| <span data-ttu-id="3d50c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d50c-110">Property</span></span> | <span data-ttu-id="3d50c-111">型</span><span class="sxs-lookup"><span data-stu-id="3d50c-111">Type</span></span> | <span data-ttu-id="3d50c-112">説明</span><span class="sxs-lookup"><span data-stu-id="3d50c-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="3d50c-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="3d50c-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="3d50c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d50c-114">Boolean</span></span> | <span data-ttu-id="3d50c-115">この web アプリケーションが OAuth 2.0 暗黙的フローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d50c-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="3d50c-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="3d50c-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="3d50c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d50c-117">Boolean</span></span> | <span data-ttu-id="3d50c-118">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してアクセストークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d50c-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d50c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d50c-119">JSON representation</span></span>
<span data-ttu-id="3d50c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d50c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
