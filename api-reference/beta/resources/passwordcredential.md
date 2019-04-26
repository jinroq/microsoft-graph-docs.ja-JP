---
title: passwordcredential リソースの種類
description: アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。 serviceprincipal エンティティおよび application エンティティの**passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568468"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="d92b8-104">passwordcredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d92b8-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d92b8-105">アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="d92b8-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="d92b8-106">[serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d92b8-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d92b8-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d92b8-107">JSON representation</span></span>

<span data-ttu-id="d92b8-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d92b8-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d92b8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d92b8-109">Properties</span></span>
| <span data-ttu-id="d92b8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d92b8-110">Property</span></span>     | <span data-ttu-id="d92b8-111">型</span><span class="sxs-lookup"><span data-stu-id="d92b8-111">Type</span></span>   |<span data-ttu-id="d92b8-112">説明</span><span class="sxs-lookup"><span data-stu-id="d92b8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d92b8-113">customkeyidentifier</span><span class="sxs-lookup"><span data-stu-id="d92b8-113">customKeyIdentifier</span></span>|<span data-ttu-id="d92b8-114">Binary</span><span class="sxs-lookup"><span data-stu-id="d92b8-114">Binary</span></span>|            |
|<span data-ttu-id="d92b8-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d92b8-115">endDateTime</span></span>|<span data-ttu-id="d92b8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d92b8-116">DateTimeOffset</span></span>|<span data-ttu-id="d92b8-117">パスワードの有効期限が切れる日付と時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d92b8-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d92b8-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d92b8-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d92b8-119">id</span><span class="sxs-lookup"><span data-stu-id="d92b8-119">keyId</span></span>|<span data-ttu-id="d92b8-120">Guid</span><span class="sxs-lookup"><span data-stu-id="d92b8-120">Guid</span></span>|            |
|<span data-ttu-id="d92b8-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d92b8-121">startDateTime</span></span>|<span data-ttu-id="d92b8-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d92b8-122">DateTimeOffset</span></span>|<span data-ttu-id="d92b8-123">パスワードが有効になる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d92b8-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d92b8-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d92b8-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d92b8-125">secretText</span><span class="sxs-lookup"><span data-stu-id="d92b8-125">secretText</span></span>|<span data-ttu-id="d92b8-126">String</span><span class="sxs-lookup"><span data-stu-id="d92b8-126">String</span></span>| <span data-ttu-id="d92b8-127">パスワードの長さは16-64 文字でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="d92b8-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="d92b8-128">hint</span><span class="sxs-lookup"><span data-stu-id="d92b8-128">hint</span></span>|<span data-ttu-id="d92b8-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d92b8-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordcredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
