---
title: passwordCredential リソースの種類
description: アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。 ServicePrincipal エンティティおよびアプリケーション エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523149"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="08141-104">passwordCredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08141-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08141-105">アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="08141-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="08141-106">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="08141-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="08141-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08141-107">JSON representation</span></span>

<span data-ttu-id="08141-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="08141-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="08141-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08141-109">Properties</span></span>
| <span data-ttu-id="08141-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08141-110">Property</span></span>     | <span data-ttu-id="08141-111">型</span><span class="sxs-lookup"><span data-stu-id="08141-111">Type</span></span>   |<span data-ttu-id="08141-112">説明</span><span class="sxs-lookup"><span data-stu-id="08141-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08141-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="08141-113">customKeyIdentifier</span></span>|<span data-ttu-id="08141-114">Binary</span><span class="sxs-lookup"><span data-stu-id="08141-114">Binary</span></span>|            |
|<span data-ttu-id="08141-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="08141-115">endDateTime</span></span>|<span data-ttu-id="08141-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08141-116">DateTimeOffset</span></span>|<span data-ttu-id="08141-117">日付と時刻、パスワードの有効期限が切れます。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="08141-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08141-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="08141-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08141-119">キー Id</span><span class="sxs-lookup"><span data-stu-id="08141-119">keyId</span></span>|<span data-ttu-id="08141-120">Guid</span><span class="sxs-lookup"><span data-stu-id="08141-120">Guid</span></span>|            |
|<span data-ttu-id="08141-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="08141-121">startDateTime</span></span>|<span data-ttu-id="08141-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08141-122">DateTimeOffset</span></span>|<span data-ttu-id="08141-123">日付と時刻にパスワードが有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="08141-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08141-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="08141-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08141-125">secretText</span><span class="sxs-lookup"><span data-stu-id="08141-125">secretText</span></span>|<span data-ttu-id="08141-126">String</span><span class="sxs-lookup"><span data-stu-id="08141-126">String</span></span>| <span data-ttu-id="08141-127">パスワードは 16 ~ 64 文字の長さである必要があります。</span><span class="sxs-lookup"><span data-stu-id="08141-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="08141-128">ヒント</span><span class="sxs-lookup"><span data-stu-id="08141-128">hint</span></span>|<span data-ttu-id="08141-129">String</span><span class="sxs-lookup"><span data-stu-id="08141-129">String</span></span>|  |

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
