---
title: localeInfo リソースの種類
description: サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。
ms.openlocfilehash: 5dae464a4931fb094ae47cce600a95d55c6c3f93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072799"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="df86b-103">localeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df86b-103">localeInfo resource type</span></span>

> <span data-ttu-id="df86b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df86b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df86b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df86b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df86b-106">サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。</span><span class="sxs-lookup"><span data-stu-id="df86b-106">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="df86b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df86b-107">Properties</span></span>
| <span data-ttu-id="df86b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df86b-108">Property</span></span>     | <span data-ttu-id="df86b-109">型</span><span class="sxs-lookup"><span data-stu-id="df86b-109">Type</span></span>   |<span data-ttu-id="df86b-110">説明</span><span class="sxs-lookup"><span data-stu-id="df86b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df86b-111">locale</span><span class="sxs-lookup"><span data-stu-id="df86b-111">locale</span></span>|<span data-ttu-id="df86b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="df86b-112">string</span></span>|<span data-ttu-id="df86b-p102">ユーザーのロケールを表します。ユーザーの優先言語および国/地域が含まれます。たとえば、"en-us"。言語のコンポーネントは [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) で定義されている 2 文字のコードに従い、国のコンポーネントは [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) で定義されている 2 文字のコードに従います。</span><span class="sxs-lookup"><span data-stu-id="df86b-p102">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="df86b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="df86b-116">displayName</span></span>|<span data-ttu-id="df86b-117">string</span><span class="sxs-lookup"><span data-stu-id="df86b-117">string</span></span>|<span data-ttu-id="df86b-118">たとえば "English (United States)" のように、ユーザーのロケールを自然言語で表す名前。</span><span class="sxs-lookup"><span data-stu-id="df86b-118">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df86b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df86b-119">JSON representation</span></span>

<span data-ttu-id="df86b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df86b-120">Here is a JSON representation of the resource.</span></span>

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