---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
ms.openlocfilehash: 1026f3b97a3305dff7a715fae000ab9695ac8e9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333611"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="8cbfa-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cbfa-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cbfa-106">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="8cbfa-107">個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="8cbfa-108">暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="8cbfa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cbfa-109">Properties</span></span>

| <span data-ttu-id="8cbfa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cbfa-110">Property</span></span> | <span data-ttu-id="8cbfa-111">型</span><span class="sxs-lookup"><span data-stu-id="8cbfa-111">Type</span></span> | <span data-ttu-id="8cbfa-112">説明</span><span class="sxs-lookup"><span data-stu-id="8cbfa-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="8cbfa-113">enableidtokenissuance</span><span class="sxs-lookup"><span data-stu-id="8cbfa-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="8cbfa-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cbfa-114">Boolean</span></span> | <span data-ttu-id="8cbfa-115">この web アプリケーションが OAuth 2.0 暗黙的フローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="8cbfa-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="8cbfa-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="8cbfa-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cbfa-117">Boolean</span></span> | <span data-ttu-id="8cbfa-118">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してアクセストークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cbfa-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cbfa-119">JSON representation</span></span>
<span data-ttu-id="8cbfa-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cbfa-120">Here is a JSON representation of the resource.</span></span>
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
