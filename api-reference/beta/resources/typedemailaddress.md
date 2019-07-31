---
title: typedEmailAddress リソースの種類
description: 連絡先の名前、電子メールアドレス、および対応する電子メールアドレスの種類を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c5ece5d1ad1c5c38253d73353b05b94727855fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007572"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="334c9-103">typedEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="334c9-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="334c9-104">[連絡先](contact.md)の名前、電子メールアドレス、および対応する電子メールアドレスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="334c9-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="334c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="334c9-105">Properties</span></span>
| <span data-ttu-id="334c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="334c9-106">Property</span></span>     | <span data-ttu-id="334c9-107">型</span><span class="sxs-lookup"><span data-stu-id="334c9-107">Type</span></span>   |<span data-ttu-id="334c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="334c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="334c9-109">address</span><span class="sxs-lookup"><span data-stu-id="334c9-109">address</span></span>|<span data-ttu-id="334c9-110">String</span><span class="sxs-lookup"><span data-stu-id="334c9-110">String</span></span>|<span data-ttu-id="334c9-111">連絡先の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="334c9-111">The email address of a contact.</span></span>|
|<span data-ttu-id="334c9-112">name</span><span class="sxs-lookup"><span data-stu-id="334c9-112">name</span></span>|<span data-ttu-id="334c9-113">String</span><span class="sxs-lookup"><span data-stu-id="334c9-113">String</span></span>|<span data-ttu-id="334c9-114">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="334c9-114">The display name of a contact.</span></span>|
|<span data-ttu-id="334c9-115">type</span><span class="sxs-lookup"><span data-stu-id="334c9-115">type</span></span> |<span data-ttu-id="334c9-116">String</span><span class="sxs-lookup"><span data-stu-id="334c9-116">String</span></span> |<span data-ttu-id="334c9-117">電子メールアドレスの種類。</span><span class="sxs-lookup"><span data-stu-id="334c9-117">The type of email address.</span></span> <span data-ttu-id="334c9-118">可能な値は、`unknown`、`work`、`personal`、`main`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="334c9-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="334c9-119">既定値はです`unknown`。これは、**アドレス**が特定の種類として設定されていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="334c9-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="334c9-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="334c9-120">otherLabel</span></span> |<span data-ttu-id="334c9-121">String</span><span class="sxs-lookup"><span data-stu-id="334c9-121">String</span></span>  |<span data-ttu-id="334c9-122">ユーザー設定の電子メールアドレスの種類を指定\*\*\*\* し、 `other`型をに設定して、ユーザー設定文字列に**otherlabel**を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="334c9-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="334c9-123">たとえば、ボランティア活動に特定の電子メールアドレスを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="334c9-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="334c9-124">**型**をに`other`設定し、 **otherlabel**をなどのカスタム文字列に`Volunteer work`設定します。</span><span class="sxs-lookup"><span data-stu-id="334c9-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="334c9-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="334c9-125">JSON representation</span></span>

<span data-ttu-id="334c9-126">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="334c9-126">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
