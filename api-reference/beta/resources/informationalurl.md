---
title: informationalurl リソースの種類
description: アプリケーションの基本的なプロファイル情報です。
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548706"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="79341-103">informationalurl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79341-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79341-104">アプリケーションの基本的なプロファイル情報です。</span><span class="sxs-lookup"><span data-stu-id="79341-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="79341-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79341-105">Properties</span></span>

| <span data-ttu-id="79341-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79341-106">Property</span></span> | <span data-ttu-id="79341-107">型</span><span class="sxs-lookup"><span data-stu-id="79341-107">Type</span></span> | <span data-ttu-id="79341-108">説明</span><span class="sxs-lookup"><span data-stu-id="79341-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="79341-109">市場</span><span class="sxs-lookup"><span data-stu-id="79341-109">marketing</span></span>|<span data-ttu-id="79341-110">String</span><span class="sxs-lookup"><span data-stu-id="79341-110">String</span></span>| <span data-ttu-id="79341-111">アプリケーションの [マーケティング] ページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="79341-111">Link to the application's marketing page.</span></span> <span data-ttu-id="79341-112">たとえば、https://www.contoso.com/app/marketing のように指定します。</span><span class="sxs-lookup"><span data-stu-id="79341-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="79341-113">秘密</span><span class="sxs-lookup"><span data-stu-id="79341-113">privacy</span></span>|<span data-ttu-id="79341-114">String</span><span class="sxs-lookup"><span data-stu-id="79341-114">String</span></span>| <span data-ttu-id="79341-115">アプリケーションのプライバシーに関する声明にリンクします。</span><span class="sxs-lookup"><span data-stu-id="79341-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="79341-116">たとえば、https://www.contoso.com/app/privacy のように指定します。</span><span class="sxs-lookup"><span data-stu-id="79341-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="79341-117">・</span><span class="sxs-lookup"><span data-stu-id="79341-117">support</span></span>|<span data-ttu-id="79341-118">String</span><span class="sxs-lookup"><span data-stu-id="79341-118">String</span></span>| <span data-ttu-id="79341-119">アプリケーションのサポートページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="79341-119">Link to the application's support page.</span></span> <span data-ttu-id="79341-120">たとえば、https://www.contoso.com/app/support のように指定します。</span><span class="sxs-lookup"><span data-stu-id="79341-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="79341-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="79341-121">termsOfService</span></span>|<span data-ttu-id="79341-122">String</span><span class="sxs-lookup"><span data-stu-id="79341-122">String</span></span>| <span data-ttu-id="79341-123">アプリケーションのサービス条件ステートメントにリンクします。</span><span class="sxs-lookup"><span data-stu-id="79341-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="79341-124">たとえば、https://www.contoso.com/app/termsofservice のように指定します。</span><span class="sxs-lookup"><span data-stu-id="79341-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79341-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79341-125">JSON representation</span></span>
<span data-ttu-id="79341-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79341-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
