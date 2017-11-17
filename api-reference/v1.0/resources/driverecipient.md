---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 53f6a5559cb90142a88b839a996cb2eedfd1037a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="driverecipient-resource"></a><span data-ttu-id="74f8f-102">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="74f8f-102">DriveRecipient resource type</span></span>

<span data-ttu-id="74f8f-103">**DriveRecipient** リソースは、[出席依頼](../api/driveitem_invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="74f8f-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem_invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74f8f-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74f8f-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="74f8f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f8f-105">Properties</span></span>
<span data-ttu-id="74f8f-106">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="74f8f-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="74f8f-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="74f8f-107">Property name</span></span> | <span data-ttu-id="74f8f-108">種類</span><span class="sxs-lookup"><span data-stu-id="74f8f-108">Type</span></span>   | <span data-ttu-id="74f8f-109">説明</span><span class="sxs-lookup"><span data-stu-id="74f8f-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="74f8f-110">email</span><span class="sxs-lookup"><span data-stu-id="74f8f-110">email</span></span>         | <span data-ttu-id="74f8f-111">String</span><span class="sxs-lookup"><span data-stu-id="74f8f-111">String</span></span> | <span data-ttu-id="74f8f-112">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="74f8f-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="74f8f-113">alias</span><span class="sxs-lookup"><span data-stu-id="74f8f-113">alias</span></span>         | <span data-ttu-id="74f8f-114">String</span><span class="sxs-lookup"><span data-stu-id="74f8f-114">String</span></span> | <span data-ttu-id="74f8f-115">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="74f8f-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="74f8f-116">objectId</span><span class="sxs-lookup"><span data-stu-id="74f8f-116">objectId</span></span>      | <span data-ttu-id="74f8f-117">String</span><span class="sxs-lookup"><span data-stu-id="74f8f-117">String</span></span> | <span data-ttu-id="74f8f-118">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="74f8f-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="74f8f-119">注釈</span><span class="sxs-lookup"><span data-stu-id="74f8f-119">Remarks</span></span>

<span data-ttu-id="74f8f-120">[出席依頼](../api/driveitem_invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。</span><span class="sxs-lookup"><span data-stu-id="74f8f-120">When using invite to add permissions, the DriveRecipient can specify email, alias, or objectId. Only one of these values is required.</span></span>
<span data-ttu-id="74f8f-121">これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="74f8f-121">Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
