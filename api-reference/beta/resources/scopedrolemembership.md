---
title: scopedRoleMembership リソースの種類
description: スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。  これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。
localization_priority: Normal
ms.openlocfilehash: c3af7a44221c4cf2822440a6025706c8bd4a93ac
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575661"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="d0de1-104">scopedRoleMembership リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0de1-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0de1-105">スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d0de1-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="d0de1-106">これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。</span><span class="sxs-lookup"><span data-stu-id="d0de1-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="d0de1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0de1-107">Methods</span></span>
<span data-ttu-id="d0de1-108">このリソースへの直接のクエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0de1-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="d0de1-109">スコープ ロール メンバーシップの追加と削除と同様にスコープ ロールのメンバーシップを照会する方法についての情報を表示する[単位数の管理](administrativeunit.md)トピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0de1-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="d0de1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0de1-110">Properties</span></span>
| <span data-ttu-id="d0de1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0de1-111">Property</span></span>   | <span data-ttu-id="d0de1-112">型</span><span class="sxs-lookup"><span data-stu-id="d0de1-112">Type</span></span> | <span data-ttu-id="d0de1-113">説明</span><span class="sxs-lookup"><span data-stu-id="d0de1-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d0de1-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="d0de1-114">administrativeUnitId</span></span>|<span data-ttu-id="d0de1-115">文字列</span><span class="sxs-lookup"><span data-stu-id="d0de1-115">string</span></span>|<span data-ttu-id="d0de1-116">ディレクトリの役割のスコープは、管理単位の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="d0de1-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="d0de1-117">id</span><span class="sxs-lookup"><span data-stu-id="d0de1-117">id</span></span>|<span data-ttu-id="d0de1-118">文字列</span><span class="sxs-lookup"><span data-stu-id="d0de1-118">string</span></span>| <span data-ttu-id="d0de1-119">スコープ ロール メンバーシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d0de1-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="d0de1-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d0de1-120">Read-only.</span></span>|
|<span data-ttu-id="d0de1-121">roleId</span><span class="sxs-lookup"><span data-stu-id="d0de1-121">roleId</span></span>|<span data-ttu-id="d0de1-122">文字列</span><span class="sxs-lookup"><span data-stu-id="d0de1-122">string</span></span>| <span data-ttu-id="d0de1-123">メンバーが含まれるディレクトリの役割の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d0de1-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="d0de1-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="d0de1-124">roleMemberInfo</span></span>|[<span data-ttu-id="d0de1-125">identity</span><span class="sxs-lookup"><span data-stu-id="d0de1-125">identity</span></span>](identity.md)| <span data-ttu-id="d0de1-126">ロール メンバーの識別情報です。</span><span class="sxs-lookup"><span data-stu-id="d0de1-126">Role member identity information.</span></span> <span data-ttu-id="d0de1-127">このスコープの役割のメンバーであるユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="d0de1-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0de1-128">関係</span><span class="sxs-lookup"><span data-stu-id="d0de1-128">Relationships</span></span>
<span data-ttu-id="d0de1-129">なし</span><span class="sxs-lookup"><span data-stu-id="d0de1-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d0de1-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0de1-130">JSON representation</span></span>

<span data-ttu-id="d0de1-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0de1-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
