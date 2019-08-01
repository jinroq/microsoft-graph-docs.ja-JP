---
title: localeInfo リソースの種類
description: サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c9ee379e76c709f48b8dcf4ea9e706126b957525
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036436"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="34e20-103">localeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34e20-103">localeInfo resource type</span></span>

<span data-ttu-id="34e20-104">サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。</span><span class="sxs-lookup"><span data-stu-id="34e20-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="34e20-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34e20-105">Properties</span></span>
| <span data-ttu-id="34e20-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34e20-106">Property</span></span>     | <span data-ttu-id="34e20-107">型</span><span class="sxs-lookup"><span data-stu-id="34e20-107">Type</span></span>   |<span data-ttu-id="34e20-108">説明</span><span class="sxs-lookup"><span data-stu-id="34e20-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34e20-109">locale</span><span class="sxs-lookup"><span data-stu-id="34e20-109">locale</span></span>|<span data-ttu-id="34e20-110">string</span><span class="sxs-lookup"><span data-stu-id="34e20-110">string</span></span>|<span data-ttu-id="34e20-p101">ユーザーのロケールを表します。ユーザーの優先言語および国/地域が含まれます。たとえば、"en-us"。言語のコンポーネントは [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) で定義されている 2 文字のコードに従い、国のコンポーネントは [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) で定義されている 2 文字のコードに従います。</span><span class="sxs-lookup"><span data-stu-id="34e20-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="34e20-114">displayName</span><span class="sxs-lookup"><span data-stu-id="34e20-114">displayName</span></span>|<span data-ttu-id="34e20-115">string</span><span class="sxs-lookup"><span data-stu-id="34e20-115">string</span></span>|<span data-ttu-id="34e20-116">たとえば "English (United States)" のように、ユーザーのロケールを自然言語で表す名前。</span><span class="sxs-lookup"><span data-stu-id="34e20-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34e20-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34e20-117">JSON representation</span></span>

<span data-ttu-id="34e20-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34e20-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
