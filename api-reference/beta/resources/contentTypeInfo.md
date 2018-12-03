---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070791"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="9a5b6-102">ContentTypeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a5b6-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="9a5b6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a5b6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a5b6-105">**ContentTypeInfo** リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a5b6-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a5b6-106">JSON representation</span></span>

<span data-ttu-id="9a5b6-107">以下は、**contentTypeInfo** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="9a5b6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a5b6-108">Properties</span></span>

| <span data-ttu-id="9a5b6-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9a5b6-109">Property name</span></span>  | <span data-ttu-id="9a5b6-110">型</span><span class="sxs-lookup"><span data-stu-id="9a5b6-110">Type</span></span>    | <span data-ttu-id="9a5b6-111">説明</span><span class="sxs-lookup"><span data-stu-id="9a5b6-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="9a5b6-112">**id**</span><span class="sxs-lookup"><span data-stu-id="9a5b6-112">**id**</span></span>         | <span data-ttu-id="9a5b6-113">string</span><span class="sxs-lookup"><span data-stu-id="9a5b6-113">string</span></span>  | <span data-ttu-id="9a5b6-114">コンテンツ タイプの ID。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-114">The id of the content type.</span></span>
| <span data-ttu-id="9a5b6-115">**name**</span><span class="sxs-lookup"><span data-stu-id="9a5b6-115">**name**</span></span>       | <span data-ttu-id="9a5b6-116">文字列</span><span class="sxs-lookup"><span data-stu-id="9a5b6-116">string</span></span>  | <span data-ttu-id="9a5b6-117">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="9a5b6-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
