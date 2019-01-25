---
title: keyCredential リソースの種類
description: アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。 アプリケーションと servicePrincipal のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519053"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="473cd-104">keyCredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="473cd-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473cd-105">アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="473cd-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="473cd-106">[アプリケーション](application.md)と[servicePrincipal](serviceprincipal.md)のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="473cd-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="473cd-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="473cd-107">JSON representation</span></span>

<span data-ttu-id="473cd-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="473cd-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="473cd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="473cd-109">Properties</span></span>
| <span data-ttu-id="473cd-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="473cd-110">Property</span></span>     | <span data-ttu-id="473cd-111">型</span><span class="sxs-lookup"><span data-stu-id="473cd-111">Type</span></span>   |<span data-ttu-id="473cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="473cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="473cd-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="473cd-113">customKeyIdentifier</span></span>|<span data-ttu-id="473cd-114">Binary</span><span class="sxs-lookup"><span data-stu-id="473cd-114">Binary</span></span>| <span data-ttu-id="473cd-115">カスタム キー識別子</span><span class="sxs-lookup"><span data-stu-id="473cd-115">Custom key identifier</span></span> |
|<span data-ttu-id="473cd-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="473cd-116">endDateTime</span></span>|<span data-ttu-id="473cd-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="473cd-117">DateTimeOffset</span></span>|<span data-ttu-id="473cd-118">日付と、資格情報の有効期限が切れる。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="473cd-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="473cd-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="473cd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="473cd-120">キー Id</span><span class="sxs-lookup"><span data-stu-id="473cd-120">keyId</span></span>|<span data-ttu-id="473cd-121">Guid</span><span class="sxs-lookup"><span data-stu-id="473cd-121">Guid</span></span>|<span data-ttu-id="473cd-122">キーの一意の識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="473cd-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="473cd-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="473cd-123">startDateTime</span></span>|<span data-ttu-id="473cd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="473cd-124">DateTimeOffset</span></span>|<span data-ttu-id="473cd-125">日付と時刻に、資格情報が有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="473cd-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="473cd-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="473cd-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="473cd-127">type</span><span class="sxs-lookup"><span data-stu-id="473cd-127">type</span></span>|<span data-ttu-id="473cd-128">String</span><span class="sxs-lookup"><span data-stu-id="473cd-128">String</span></span>|<span data-ttu-id="473cd-129">キーの資格情報の種類「対称」などです。</span><span class="sxs-lookup"><span data-stu-id="473cd-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="473cd-130">使用状況</span><span class="sxs-lookup"><span data-stu-id="473cd-130">usage</span></span>|<span data-ttu-id="473cd-131">String</span><span class="sxs-lookup"><span data-stu-id="473cd-131">String</span></span>|<span data-ttu-id="473cd-132">キーが使われることができます; 目的を説明する文字列などの検証」です。</span><span class="sxs-lookup"><span data-stu-id="473cd-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="473cd-133">key</span><span class="sxs-lookup"><span data-stu-id="473cd-133">key</span></span>|<span data-ttu-id="473cd-134">Binary</span><span class="sxs-lookup"><span data-stu-id="473cd-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keycredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
