---
title: chatMessageMention リソースの種類
description: 'ChatMessage エンティティの参照を表します。 ユーザー、チーム、ボットまたはチャネルをことができます。 '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515350"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="f3bb1-104">chatMessageMention リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3bb1-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3bb1-105">[ChatMessage](chatmessage.md)エンティティの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="f3bb1-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="f3bb1-106">ユーザー、チーム、ボットまたはチャネルをことができます。</span><span class="sxs-lookup"><span data-stu-id="f3bb1-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="f3bb1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bb1-107">Properties</span></span>
| <span data-ttu-id="f3bb1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bb1-108">Property</span></span>     | <span data-ttu-id="f3bb1-109">型</span><span class="sxs-lookup"><span data-stu-id="f3bb1-109">Type</span></span>   |<span data-ttu-id="f3bb1-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3bb1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3bb1-111">id</span><span class="sxs-lookup"><span data-stu-id="f3bb1-111">id</span></span>|<span data-ttu-id="f3bb1-112">string</span><span class="sxs-lookup"><span data-stu-id="f3bb1-112">string</span></span>|<span data-ttu-id="f3bb1-113">記載されているエンティティの id</span><span class="sxs-lookup"><span data-stu-id="f3bb1-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="f3bb1-114">MentionText</span><span class="sxs-lookup"><span data-stu-id="f3bb1-114">mentionText</span></span>|<span data-ttu-id="f3bb1-115">string</span><span class="sxs-lookup"><span data-stu-id="f3bb1-115">string</span></span>|<span data-ttu-id="f3bb1-116">Ex の説明を表すために使用する文字列: ユーザーの表示名、チーム名等</span><span class="sxs-lookup"><span data-stu-id="f3bb1-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="f3bb1-117">Mentioned</span><span class="sxs-lookup"><span data-stu-id="f3bb1-117">mentioned</span></span>|[<span data-ttu-id="f3bb1-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="f3bb1-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="f3bb1-119">記載されているユーザー</span><span class="sxs-lookup"><span data-stu-id="f3bb1-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3bb1-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3bb1-120">JSON representation</span></span>

<span data-ttu-id="f3bb1-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3bb1-121">The following is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
