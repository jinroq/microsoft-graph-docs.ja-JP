---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 24d06c43af0d8c319ca88062c1d564648176cd30
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021531"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="58cc2-102">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="58cc2-102">DriveRecipient resource</span></span>

<span data-ttu-id="58cc2-103">**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="58cc2-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="58cc2-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58cc2-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="58cc2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58cc2-105">Properties</span></span>
<span data-ttu-id="58cc2-106">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="58cc2-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="58cc2-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="58cc2-107">Property name</span></span> | <span data-ttu-id="58cc2-108">種類</span><span class="sxs-lookup"><span data-stu-id="58cc2-108">Type</span></span>   | <span data-ttu-id="58cc2-109">説明</span><span class="sxs-lookup"><span data-stu-id="58cc2-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="58cc2-110">email</span><span class="sxs-lookup"><span data-stu-id="58cc2-110">email</span></span>         | <span data-ttu-id="58cc2-111">String</span><span class="sxs-lookup"><span data-stu-id="58cc2-111">String</span></span> | <span data-ttu-id="58cc2-112">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="58cc2-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="58cc2-113">alias</span><span class="sxs-lookup"><span data-stu-id="58cc2-113">alias</span></span>         | <span data-ttu-id="58cc2-114">String</span><span class="sxs-lookup"><span data-stu-id="58cc2-114">String</span></span> | <span data-ttu-id="58cc2-115">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="58cc2-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="58cc2-116">objectId</span><span class="sxs-lookup"><span data-stu-id="58cc2-116">objectId</span></span>      | <span data-ttu-id="58cc2-117">String</span><span class="sxs-lookup"><span data-stu-id="58cc2-117">String</span></span> | <span data-ttu-id="58cc2-118">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="58cc2-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="58cc2-119">注釈</span><span class="sxs-lookup"><span data-stu-id="58cc2-119">Remarks</span></span>

<span data-ttu-id="58cc2-p101">[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="58cc2-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
