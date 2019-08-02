---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
description: DriveRecipient リソースは、出席依頼アクションを使用して共有する個人、グループ、または他の受信者を表します。
doc_type: resourcePageType
ms.openlocfilehash: a198bdc8a50fdb754ba8f9c88ce8e925c548a600
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029387"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="b1984-103">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="b1984-103">DriveRecipient resource</span></span>

<span data-ttu-id="b1984-104">**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="b1984-104">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1984-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1984-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b1984-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1984-106">Properties</span></span>
<span data-ttu-id="b1984-107">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="b1984-107">The recipients resource has these properties.</span></span>

| <span data-ttu-id="b1984-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b1984-108">Property name</span></span> | <span data-ttu-id="b1984-109">種類</span><span class="sxs-lookup"><span data-stu-id="b1984-109">Type</span></span>   | <span data-ttu-id="b1984-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1984-110">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b1984-111">メール</span><span class="sxs-lookup"><span data-stu-id="b1984-111">email</span></span>         | <span data-ttu-id="b1984-112">String</span><span class="sxs-lookup"><span data-stu-id="b1984-112">String</span></span> | <span data-ttu-id="b1984-113">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b1984-113">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="b1984-114">alias</span><span class="sxs-lookup"><span data-stu-id="b1984-114">alias</span></span>         | <span data-ttu-id="b1984-115">String</span><span class="sxs-lookup"><span data-stu-id="b1984-115">String</span></span> | <span data-ttu-id="b1984-116">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="b1984-116">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="b1984-117">objectId</span><span class="sxs-lookup"><span data-stu-id="b1984-117">objectId</span></span>      | <span data-ttu-id="b1984-118">String</span><span class="sxs-lookup"><span data-stu-id="b1984-118">String</span></span> | <span data-ttu-id="b1984-119">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b1984-119">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="b1984-120">注釈</span><span class="sxs-lookup"><span data-stu-id="b1984-120">Remarks</span></span>

<span data-ttu-id="b1984-p101">[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="b1984-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
