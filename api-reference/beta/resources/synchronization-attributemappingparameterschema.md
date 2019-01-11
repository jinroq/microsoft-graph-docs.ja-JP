---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される 1 つのパラメーターについて説明します。
localization_priority: Normal
ms.openlocfilehash: 083f89ebc5a74e6fd58a33925b2bfa46801b7961
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892170"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="8ef05-103">attributeMappingParameterSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ef05-103">attributeMappingParameterSchema resource type</span></span>

> <span data-ttu-id="8ef05-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ef05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ef05-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ef05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ef05-106">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される 1 つのパラメーターについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8ef05-106">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8ef05-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ef05-107">Properties</span></span>

| <span data-ttu-id="8ef05-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ef05-108">Property</span></span>                   | <span data-ttu-id="8ef05-109">種類</span><span class="sxs-lookup"><span data-stu-id="8ef05-109">Type</span></span>                      | <span data-ttu-id="8ef05-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ef05-110">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="8ef05-111">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="8ef05-111">allowMultipleOccurrences</span></span>    |<span data-ttu-id="8ef05-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="8ef05-112">Boolean</span></span>                   |<span data-ttu-id="8ef05-113">複数回指定したパラメーターを提供することができます (などの文字列を複数の入力、`Concatenate(string,string,...)`関数)。</span><span class="sxs-lookup"><span data-stu-id="8ef05-113">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="8ef05-114">名前</span><span class="sxs-lookup"><span data-stu-id="8ef05-114">name</span></span>                        |<span data-ttu-id="8ef05-115">String</span><span class="sxs-lookup"><span data-stu-id="8ef05-115">String</span></span>                    |<span data-ttu-id="8ef05-116">パラメーターの名前です。</span><span class="sxs-lookup"><span data-stu-id="8ef05-116">Parameter name.</span></span> |
|<span data-ttu-id="8ef05-117">必須</span><span class="sxs-lookup"><span data-stu-id="8ef05-117">required</span></span>                    |<span data-ttu-id="8ef05-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="8ef05-118">Boolean</span></span>                   |<span data-ttu-id="8ef05-119">`true`場合は、パラメーターが必要です。それ以外の場合`false`。</span><span class="sxs-lookup"><span data-stu-id="8ef05-119">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="8ef05-120">type</span><span class="sxs-lookup"><span data-stu-id="8ef05-120">type</span></span>                        |<span data-ttu-id="8ef05-121">String</span><span class="sxs-lookup"><span data-stu-id="8ef05-121">String</span></span>                    |<span data-ttu-id="8ef05-122">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="8ef05-122">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="8ef05-123">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="8ef05-123">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ef05-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ef05-124">JSON representation</span></span>

<span data-ttu-id="8ef05-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ef05-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
