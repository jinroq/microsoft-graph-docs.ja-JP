---
title: informationalUrl リソースの種類
description: アプリケーションの基本的なプロファイル情報です。
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071532"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="a8c08-103">informationalUrl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8c08-103">informationalUrl resource type</span></span>

> <span data-ttu-id="a8c08-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a8c08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8c08-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8c08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8c08-106">アプリケーションの基本的なプロファイル情報です。</span><span class="sxs-lookup"><span data-stu-id="a8c08-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="a8c08-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8c08-107">Properties</span></span>

| <span data-ttu-id="a8c08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8c08-108">Property</span></span> | <span data-ttu-id="a8c08-109">型</span><span class="sxs-lookup"><span data-stu-id="a8c08-109">Type</span></span> | <span data-ttu-id="a8c08-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8c08-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8c08-111">マーケティング</span><span class="sxs-lookup"><span data-stu-id="a8c08-111">marketing</span></span>|<span data-ttu-id="a8c08-112">String</span><span class="sxs-lookup"><span data-stu-id="a8c08-112">String</span></span>| <span data-ttu-id="a8c08-113">アプリケーションのマーケティングのページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="a8c08-113">Link to the application's marketing page.</span></span> <span data-ttu-id="a8c08-114">たとえば、https://www.contoso.com/app/marketing では、</span><span class="sxs-lookup"><span data-stu-id="a8c08-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="a8c08-115">プライバシー</span><span class="sxs-lookup"><span data-stu-id="a8c08-115">privacy</span></span>|<span data-ttu-id="a8c08-116">String</span><span class="sxs-lookup"><span data-stu-id="a8c08-116">String</span></span>| <span data-ttu-id="a8c08-117">アプリケーションのプライバシーに関する声明へのリンクです。</span><span class="sxs-lookup"><span data-stu-id="a8c08-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="a8c08-118">たとえば、https://www.contoso.com/app/privacy では、</span><span class="sxs-lookup"><span data-stu-id="a8c08-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="a8c08-119">サポート</span><span class="sxs-lookup"><span data-stu-id="a8c08-119">support</span></span>|<span data-ttu-id="a8c08-120">String</span><span class="sxs-lookup"><span data-stu-id="a8c08-120">String</span></span>| <span data-ttu-id="a8c08-121">アプリケーションのサポートのページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="a8c08-121">Link to the application's support page.</span></span> <span data-ttu-id="a8c08-122">たとえば、https://www.contoso.com/app/support では、</span><span class="sxs-lookup"><span data-stu-id="a8c08-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="a8c08-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="a8c08-123">termsOfService</span></span>|<span data-ttu-id="a8c08-124">String</span><span class="sxs-lookup"><span data-stu-id="a8c08-124">String</span></span>| <span data-ttu-id="a8c08-125">サービスのステートメントのアプリケーションの条件にリンクします。</span><span class="sxs-lookup"><span data-stu-id="a8c08-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="a8c08-126">たとえば、https://www.contoso.com/app/termsofservice では、</span><span class="sxs-lookup"><span data-stu-id="a8c08-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8c08-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8c08-127">JSON representation</span></span>
<span data-ttu-id="a8c08-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8c08-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->