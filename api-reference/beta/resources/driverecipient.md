---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 47a080b4f81645cfe5098ec8391d58cf07fca466
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482344"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="34f8e-102">DriveRecipient リソース</span><span class="sxs-lookup"><span data-stu-id="34f8e-102">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34f8e-103">**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="34f8e-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34f8e-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34f8e-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="34f8e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34f8e-105">Properties</span></span>
<span data-ttu-id="34f8e-106">受信者のリソースには、これらのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="34f8e-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="34f8e-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="34f8e-107">Property name</span></span> | <span data-ttu-id="34f8e-108">種類</span><span class="sxs-lookup"><span data-stu-id="34f8e-108">Type</span></span>   | <span data-ttu-id="34f8e-109">説明</span><span class="sxs-lookup"><span data-stu-id="34f8e-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="34f8e-110">email</span><span class="sxs-lookup"><span data-stu-id="34f8e-110">email</span></span>         | <span data-ttu-id="34f8e-111">String
</span><span class="sxs-lookup"><span data-stu-id="34f8e-111">String</span></span> | <span data-ttu-id="34f8e-112">受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="34f8e-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="34f8e-113">alias</span><span class="sxs-lookup"><span data-stu-id="34f8e-113">alias</span></span>         | <span data-ttu-id="34f8e-114">String</span><span class="sxs-lookup"><span data-stu-id="34f8e-114">String</span></span> | <span data-ttu-id="34f8e-115">電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。</span><span class="sxs-lookup"><span data-stu-id="34f8e-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="34f8e-116">objectId</span><span class="sxs-lookup"><span data-stu-id="34f8e-116">objectId</span></span>      | <span data-ttu-id="34f8e-117">String</span><span class="sxs-lookup"><span data-stu-id="34f8e-117">String</span></span> | <span data-ttu-id="34f8e-118">ディレクトリ内の受信者の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="34f8e-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="34f8e-119">注釈</span><span class="sxs-lookup"><span data-stu-id="34f8e-119">Remarks</span></span>

<span data-ttu-id="34f8e-p101">[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。</span><span class="sxs-lookup"><span data-stu-id="34f8e-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": [
    "Error: /api-reference/beta/resources/driverecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
