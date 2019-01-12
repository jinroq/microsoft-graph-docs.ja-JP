---
title: plannerUserIds リソースの種類
description: '**PlannerUserIds**リソースは、plan を共有するユーザー ID のリストを表します。これはオープン型です。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、グループの計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 150e36910da5ed6bc8c3eccd3647f487a1e3438e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984746"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="a6741-106">plannerUserIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6741-106">plannerUserIds resource type</span></span>

> <span data-ttu-id="a6741-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6741-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6741-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6741-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6741-p103">**PlannerUserIds**リソースは、[plan](plannerplan.md) を共有するユーザー ID のリストを表します。これはオープン型です。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="a6741-p103">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with. This is an Open Type. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="a6741-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6741-113">Properties</span></span>
<span data-ttu-id="a6741-p104">クライアントは、オープン型のプロパティを定義できます。この例では、クライアントは、値が `true` ブール値となるプロパティとしてユーザー ID を指定する必要があります。ユーザー ID が共有されなくなると、プロパティはその値が `false` ブール値に設定され、自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="a6741-p104">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a6741-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6741-117">JSON representation</span></span>

<span data-ttu-id="a6741-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a6741-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="a6741-119">// 例</span><span class="sxs-lookup"><span data-stu-id="a6741-119">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
