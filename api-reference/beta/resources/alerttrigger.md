---
title: alerttrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: cda1dde9b22b9304fd412405758435be2f6143bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535699"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="4f7e8-104">alerttrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f7e8-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f7e8-105">検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="4f7e8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f7e8-106">Properties</span></span>

| <span data-ttu-id="4f7e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f7e8-107">Property</span></span>   | <span data-ttu-id="4f7e8-108">型</span><span class="sxs-lookup"><span data-stu-id="4f7e8-108">Type</span></span>|<span data-ttu-id="4f7e8-109">説明</span><span class="sxs-lookup"><span data-stu-id="4f7e8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f7e8-110">name</span><span class="sxs-lookup"><span data-stu-id="4f7e8-110">name</span></span>|<span data-ttu-id="4f7e8-111">String</span><span class="sxs-lookup"><span data-stu-id="4f7e8-111">String</span></span>|<span data-ttu-id="4f7e8-112">検出トリガーとして機能するプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="4f7e8-113">type</span><span class="sxs-lookup"><span data-stu-id="4f7e8-113">type</span></span>|<span data-ttu-id="4f7e8-114">String</span><span class="sxs-lookup"><span data-stu-id="4f7e8-114">String</span></span>|<span data-ttu-id="4f7e8-115">キーと値のペアで解釈するプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="4f7e8-116">たとえば、String、Boolean、などです。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="4f7e8-117">value</span><span class="sxs-lookup"><span data-stu-id="4f7e8-117">value</span></span>|<span data-ttu-id="4f7e8-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4f7e8-118">String</span></span>|<span data-ttu-id="4f7e8-119">検出トリガーとして提供されるプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f7e8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f7e8-120">JSON representation</span></span>

<span data-ttu-id="4f7e8-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f7e8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="4f7e8-122">例</span><span class="sxs-lookup"><span data-stu-id="4f7e8-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alerttrigger.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
