---
title: informationalUrl リソースの種類
description: アプリケーションの基本的なプロファイル情報です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006256"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="e14cf-103">informationalUrl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e14cf-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e14cf-104">アプリケーションの基本的なプロファイル情報です。</span><span class="sxs-lookup"><span data-stu-id="e14cf-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="e14cf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e14cf-105">Properties</span></span>

| <span data-ttu-id="e14cf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e14cf-106">Property</span></span> | <span data-ttu-id="e14cf-107">型</span><span class="sxs-lookup"><span data-stu-id="e14cf-107">Type</span></span> | <span data-ttu-id="e14cf-108">説明</span><span class="sxs-lookup"><span data-stu-id="e14cf-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e14cf-109">市場</span><span class="sxs-lookup"><span data-stu-id="e14cf-109">marketing</span></span>|<span data-ttu-id="e14cf-110">String</span><span class="sxs-lookup"><span data-stu-id="e14cf-110">String</span></span>| <span data-ttu-id="e14cf-111">アプリケーションの [マーケティング] ページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="e14cf-111">Link to the application's marketing page.</span></span> <span data-ttu-id="e14cf-112">たとえば、https://www.contoso.com/app/marketing のように指定します。</span><span class="sxs-lookup"><span data-stu-id="e14cf-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="e14cf-113">秘密</span><span class="sxs-lookup"><span data-stu-id="e14cf-113">privacy</span></span>|<span data-ttu-id="e14cf-114">String</span><span class="sxs-lookup"><span data-stu-id="e14cf-114">String</span></span>| <span data-ttu-id="e14cf-115">アプリケーションのプライバシーに関する声明にリンクします。</span><span class="sxs-lookup"><span data-stu-id="e14cf-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="e14cf-116">たとえば、https://www.contoso.com/app/privacy のように指定します。</span><span class="sxs-lookup"><span data-stu-id="e14cf-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="e14cf-117">・</span><span class="sxs-lookup"><span data-stu-id="e14cf-117">support</span></span>|<span data-ttu-id="e14cf-118">String</span><span class="sxs-lookup"><span data-stu-id="e14cf-118">String</span></span>| <span data-ttu-id="e14cf-119">アプリケーションのサポートページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="e14cf-119">Link to the application's support page.</span></span> <span data-ttu-id="e14cf-120">たとえば、https://www.contoso.com/app/support のように指定します。</span><span class="sxs-lookup"><span data-stu-id="e14cf-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="e14cf-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="e14cf-121">termsOfService</span></span>|<span data-ttu-id="e14cf-122">String</span><span class="sxs-lookup"><span data-stu-id="e14cf-122">String</span></span>| <span data-ttu-id="e14cf-123">アプリケーションのサービス条件ステートメントにリンクします。</span><span class="sxs-lookup"><span data-stu-id="e14cf-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="e14cf-124">たとえば、https://www.contoso.com/app/termsofservice のように指定します。</span><span class="sxs-lookup"><span data-stu-id="e14cf-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e14cf-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e14cf-125">JSON representation</span></span>
<span data-ttu-id="e14cf-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e14cf-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
