---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c1a121969bf6b36c8afccd367a084a4b75599eaf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334608"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="001d3-102">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="001d3-102">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001d3-103">**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="001d3-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="001d3-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="001d3-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="001d3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="001d3-105">Properties</span></span>
<span data-ttu-id="001d3-106">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="001d3-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="001d3-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="001d3-107">Property name</span></span> | <span data-ttu-id="001d3-108">種類</span><span class="sxs-lookup"><span data-stu-id="001d3-108">Type</span></span>   | <span data-ttu-id="001d3-109">説明</span><span class="sxs-lookup"><span data-stu-id="001d3-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="001d3-110">email</span><span class="sxs-lookup"><span data-stu-id="001d3-110">email</span></span>         | <span data-ttu-id="001d3-111">String</span><span class="sxs-lookup"><span data-stu-id="001d3-111">String</span></span> | <span data-ttu-id="001d3-112">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="001d3-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="001d3-113">alias</span><span class="sxs-lookup"><span data-stu-id="001d3-113">alias</span></span>         | <span data-ttu-id="001d3-114">String</span><span class="sxs-lookup"><span data-stu-id="001d3-114">String</span></span> | <span data-ttu-id="001d3-115">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="001d3-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="001d3-116">objectId</span><span class="sxs-lookup"><span data-stu-id="001d3-116">objectId</span></span>      | <span data-ttu-id="001d3-117">String</span><span class="sxs-lookup"><span data-stu-id="001d3-117">String</span></span> | <span data-ttu-id="001d3-118">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="001d3-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="001d3-119">注釈</span><span class="sxs-lookup"><span data-stu-id="001d3-119">Remarks</span></span>

<span data-ttu-id="001d3-p101">[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="001d3-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

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
