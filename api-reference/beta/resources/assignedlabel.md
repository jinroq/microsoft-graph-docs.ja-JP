---
title: assignedLabel リソースの種類
description: Office 365 グループに割り当てられた機密ラベルを表します。 機密ラベルを使用すると、管理者はグループに分類を割り当てることにより、グループに特定のグループ設定を適用することができます (機密、高機密、一般)。
localization_priority: Normal
author: krbain
ms.prod: groups
ms.openlocfilehash: 430387f228bf632a7f9f9b4a046537bbe5ff4953
ms.sourcegitcommit: b18ccb24fc79f3abb470cd759e25cdd266fc77c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/17/2019
ms.locfileid: "34117621"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="30b7a-104">assignedLabel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30b7a-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30b7a-105">Office 365 グループに割り当てられた機密ラベルを表します。</span><span class="sxs-lookup"><span data-stu-id="30b7a-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="30b7a-106">機密ラベルを使用すると、管理者はグループに分類を割り当てることにより、グループに特定のグループ設定を適用することができます (機密、高機密、一般)。</span><span class="sxs-lookup"><span data-stu-id="30b7a-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="30b7a-107">機密ラベルは microsoft 365 Security & コンプライアンスセンターの管理者によって、Microsoft Information Protection 機能の一部として公開されています。</span><span class="sxs-lookup"><span data-stu-id="30b7a-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="30b7a-108">機密ラベルの詳細については、「[感度ラベルの概要](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30b7a-108">For more information about sensitivity labels, see [Sensitivity labels overview](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="30b7a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30b7a-109">Properties</span></span>
| <span data-ttu-id="30b7a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30b7a-110">Property</span></span>     | <span data-ttu-id="30b7a-111">型</span><span class="sxs-lookup"><span data-stu-id="30b7a-111">Type</span></span>   |<span data-ttu-id="30b7a-112">説明</span><span class="sxs-lookup"><span data-stu-id="30b7a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30b7a-113">Lab_ d</span><span class="sxs-lookup"><span data-stu-id="30b7a-113">labelId</span></span>|<span data-ttu-id="30b7a-114">String</span><span class="sxs-lookup"><span data-stu-id="30b7a-114">String</span></span>|<span data-ttu-id="30b7a-115">ラベルの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="30b7a-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="30b7a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="30b7a-116">displayName</span></span>|<span data-ttu-id="30b7a-117">String</span><span class="sxs-lookup"><span data-stu-id="30b7a-117">String</span></span>|<span data-ttu-id="30b7a-118">ラベルの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="30b7a-118">The display name of the label.</span></span> <span data-ttu-id="30b7a-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="30b7a-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30b7a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30b7a-120">JSON representation</span></span>

<span data-ttu-id="30b7a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="30b7a-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
