---
title: educationOneNoteResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、OneNote のページの場所を表します。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9dea19683786d22c48af2eedd6239ffe76441ef2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825929"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="c5b2f-104">educationOneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5b2f-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="c5b2f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5b2f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5b2f-107">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="c5b2f-108">これは、OneNote のページの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="c5b2f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5b2f-109">Properties</span></span>
| <span data-ttu-id="c5b2f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5b2f-110">Property</span></span>     | <span data-ttu-id="c5b2f-111">種類</span><span class="sxs-lookup"><span data-stu-id="c5b2f-111">Type</span></span>   |<span data-ttu-id="c5b2f-112">説明</span><span class="sxs-lookup"><span data-stu-id="c5b2f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5b2f-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="c5b2f-113">pageUrl</span></span>|<span data-ttu-id="c5b2f-114">String</span><span class="sxs-lookup"><span data-stu-id="c5b2f-114">String</span></span>|<span data-ttu-id="c5b2f-115">OneNote のページに Microsoft のグラフの URL です。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="c5b2f-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="c5b2f-116">sectionName</span></span>|<span data-ttu-id="c5b2f-117">String</span><span class="sxs-lookup"><span data-stu-id="c5b2f-117">String</span></span>|<span data-ttu-id="c5b2f-118">ディストリビューションにコピーする必要がありますにコピーされたセクションの名前です。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5b2f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5b2f-119">JSON representation</span></span>

<span data-ttu-id="c5b2f-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5b2f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
