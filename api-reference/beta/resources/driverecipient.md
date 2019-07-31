---
author: JeremyKelley
description: DriveRecipient リソースは、出席依頼アクションを使用して共有する個人、グループ、または他の受信者を表します。
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f86b79567b4148934f1c9624124026472fbb3395
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012710"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="72c01-103">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="72c01-103">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c01-104">**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="72c01-104">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72c01-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72c01-105">JSON representation</span></span>

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a><span data-ttu-id="72c01-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72c01-106">Properties</span></span>
<span data-ttu-id="72c01-107">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="72c01-107">The recipients resource has these properties.</span></span>

| <span data-ttu-id="72c01-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="72c01-108">Property name</span></span> | <span data-ttu-id="72c01-109">種類</span><span class="sxs-lookup"><span data-stu-id="72c01-109">Type</span></span>   | <span data-ttu-id="72c01-110">説明</span><span class="sxs-lookup"><span data-stu-id="72c01-110">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="72c01-111">メール</span><span class="sxs-lookup"><span data-stu-id="72c01-111">email</span></span>         | <span data-ttu-id="72c01-112">String</span><span class="sxs-lookup"><span data-stu-id="72c01-112">String</span></span> | <span data-ttu-id="72c01-113">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="72c01-113">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="72c01-114">alias</span><span class="sxs-lookup"><span data-stu-id="72c01-114">alias</span></span>         | <span data-ttu-id="72c01-115">String</span><span class="sxs-lookup"><span data-stu-id="72c01-115">String</span></span> | <span data-ttu-id="72c01-116">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="72c01-116">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="72c01-117">objectId</span><span class="sxs-lookup"><span data-stu-id="72c01-117">objectId</span></span>      | <span data-ttu-id="72c01-118">String</span><span class="sxs-lookup"><span data-stu-id="72c01-118">String</span></span> | <span data-ttu-id="72c01-119">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="72c01-119">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="72c01-120">注釈</span><span class="sxs-lookup"><span data-stu-id="72c01-120">Remarks</span></span>

<span data-ttu-id="72c01-p101">[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="72c01-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
