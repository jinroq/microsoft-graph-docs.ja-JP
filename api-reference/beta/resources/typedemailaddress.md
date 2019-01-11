---
title: typedEmailAddress リソースの種類
description: 名前、電子メール アドレス、および連絡先の対応する電子メール アドレス タイプを表します。
localization_priority: Normal
ms.openlocfilehash: c77d3dddc3e2bfcac47e6ed245dad9223fe7f08c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871268"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="9f209-103">typedEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f209-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="9f209-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f209-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f209-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f209-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f209-106">名前、電子メール アドレス、および、対応する電子メール アドレスの種類[にお問い合わせください](contact.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="9f209-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9f209-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f209-107">Properties</span></span>
| <span data-ttu-id="9f209-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f209-108">Property</span></span>     | <span data-ttu-id="9f209-109">種類</span><span class="sxs-lookup"><span data-stu-id="9f209-109">Type</span></span>   |<span data-ttu-id="9f209-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f209-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f209-111">address</span><span class="sxs-lookup"><span data-stu-id="9f209-111">address</span></span>|<span data-ttu-id="9f209-112">String</span><span class="sxs-lookup"><span data-stu-id="9f209-112">String</span></span>|<span data-ttu-id="9f209-113">連絡先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9f209-113">The email address of a contact.</span></span>|
|<span data-ttu-id="9f209-114">名前</span><span class="sxs-lookup"><span data-stu-id="9f209-114">name</span></span>|<span data-ttu-id="9f209-115">String</span><span class="sxs-lookup"><span data-stu-id="9f209-115">String</span></span>|<span data-ttu-id="9f209-116">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="9f209-116">The display name of a contact.</span></span>|
|<span data-ttu-id="9f209-117">type</span><span class="sxs-lookup"><span data-stu-id="9f209-117">type</span></span> |<span data-ttu-id="9f209-118">String</span><span class="sxs-lookup"><span data-stu-id="9f209-118">String</span></span> |<span data-ttu-id="9f209-119">電子メール アドレスの種類。</span><span class="sxs-lookup"><span data-stu-id="9f209-119">The type of email address.</span></span> <span data-ttu-id="9f209-120">可能な値は、`unknown`、`work`、`personal`、`main`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="9f209-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="9f209-121">既定値は、 `unknown`、つまり、**アドレス**が設定されていない特定の種類として。</span><span class="sxs-lookup"><span data-stu-id="9f209-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="9f209-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="9f209-122">otherLabel</span></span> |<span data-ttu-id="9f209-123">String</span><span class="sxs-lookup"><span data-stu-id="9f209-123">String</span></span>  |<span data-ttu-id="9f209-124">電子メール アドレスのカスタムの型を指定する**の種類**を設定`other`、 **otherLabel**を独自の文字列を割り当てるとします。</span><span class="sxs-lookup"><span data-stu-id="9f209-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="9f209-125">など、ボランティア活動の特定の電子メール アドレスを使用する場合があります。</span><span class="sxs-lookup"><span data-stu-id="9f209-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="9f209-126">**タイプ**を設定`other`、 **otherLabel**を次のように独自の文字列を設定して`Volunteer work`。</span><span class="sxs-lookup"><span data-stu-id="9f209-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f209-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f209-127">JSON representation</span></span>

<span data-ttu-id="9f209-128">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9f209-128">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
