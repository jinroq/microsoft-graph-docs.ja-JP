---
title: chatMessageMention リソースの種類
description: 'chatmessage エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 '
localization_priority: Normal
ms.openlocfilehash: 45b4c60e22f727210150a64078935741dfb71640
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481371"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="2445c-104">chatMessageMention リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2445c-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2445c-105">[chatmessage](chatmessage.md)エンティティ内のメンションを表します。</span><span class="sxs-lookup"><span data-stu-id="2445c-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="2445c-106">メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。</span><span class="sxs-lookup"><span data-stu-id="2445c-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="2445c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2445c-107">Properties</span></span>
| <span data-ttu-id="2445c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2445c-108">Property</span></span>     | <span data-ttu-id="2445c-109">型</span><span class="sxs-lookup"><span data-stu-id="2445c-109">Type</span></span>   |<span data-ttu-id="2445c-110">説明</span><span class="sxs-lookup"><span data-stu-id="2445c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2445c-111">id</span><span class="sxs-lookup"><span data-stu-id="2445c-111">id</span></span>|<span data-ttu-id="2445c-112">string</span><span class="sxs-lookup"><span data-stu-id="2445c-112">string</span></span>|<span data-ttu-id="2445c-113">記載されているエンティティの Id</span><span class="sxs-lookup"><span data-stu-id="2445c-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="2445c-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="2445c-114">mentionText</span></span>|<span data-ttu-id="2445c-115">string</span><span class="sxs-lookup"><span data-stu-id="2445c-115">string</span></span>|<span data-ttu-id="2445c-116">説明の Ex: ユーザーの表示名、チーム名などを表すために使用される文字列</span><span class="sxs-lookup"><span data-stu-id="2445c-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="2445c-117">明記</span><span class="sxs-lookup"><span data-stu-id="2445c-117">mentioned</span></span>|[<span data-ttu-id="2445c-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="2445c-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="2445c-119">説明したユーザー</span><span class="sxs-lookup"><span data-stu-id="2445c-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2445c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2445c-120">JSON representation</span></span>

<span data-ttu-id="2445c-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2445c-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
