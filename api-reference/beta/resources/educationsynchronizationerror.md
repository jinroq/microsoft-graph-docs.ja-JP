---
title: educationSynchronizationError リソースの種類
description: 学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525144"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="452a2-103">educationSynchronizationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="452a2-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="452a2-104">学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。</span><span class="sxs-lookup"><span data-stu-id="452a2-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="452a2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="452a2-105">Methods</span></span>

| <span data-ttu-id="452a2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="452a2-106">Method</span></span> | <span data-ttu-id="452a2-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="452a2-107">Return Type</span></span> | <span data-ttu-id="452a2-108">説明</span><span class="sxs-lookup"><span data-stu-id="452a2-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="452a2-109">同期エラーが発生をします。</span><span class="sxs-lookup"><span data-stu-id="452a2-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="452a2-110">**educationSynchronizationError**コレクション</span><span class="sxs-lookup"><span data-stu-id="452a2-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="452a2-111">プロファイルに関連付けられている同期エラーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="452a2-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="452a2-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="452a2-112">Properties</span></span>

| <span data-ttu-id="452a2-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="452a2-113">Property</span></span> | <span data-ttu-id="452a2-114">型</span><span class="sxs-lookup"><span data-stu-id="452a2-114">Type</span></span> | <span data-ttu-id="452a2-115">説明</span><span class="sxs-lookup"><span data-stu-id="452a2-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="452a2-116">**示した**</span><span class="sxs-lookup"><span data-stu-id="452a2-116">**entryType**</span></span> | <span data-ttu-id="452a2-117">string</span><span class="sxs-lookup"><span data-stu-id="452a2-117">string</span></span> |  <span data-ttu-id="452a2-118">(学校、セクション、学生、教師) は、同期エンティティを表します。</span><span class="sxs-lookup"><span data-stu-id="452a2-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="452a2-119">errorCode</span><span class="sxs-lookup"><span data-stu-id="452a2-119">**errorCode**</span></span> | <span data-ttu-id="452a2-120">string</span><span class="sxs-lookup"><span data-stu-id="452a2-120">string</span></span> |  <span data-ttu-id="452a2-121">このエラーのエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="452a2-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="452a2-122">**ErrorMessage**</span><span class="sxs-lookup"><span data-stu-id="452a2-122">**errorMessage**</span></span> | <span data-ttu-id="452a2-123">string</span><span class="sxs-lookup"><span data-stu-id="452a2-123">string</span></span> |  <span data-ttu-id="452a2-124">エラーの説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="452a2-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="452a2-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="452a2-125">**joiningValue**</span></span> | <span data-ttu-id="452a2-126">string</span><span class="sxs-lookup"><span data-stu-id="452a2-126">string</span></span> |  <span data-ttu-id="452a2-127">エントリの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="452a2-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="452a2-128">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="452a2-128">**recordedDateTime**</span></span> | <span data-ttu-id="452a2-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="452a2-129">DateTimeOffset</span></span> | <span data-ttu-id="452a2-130">このエラーの発生時刻。</span><span class="sxs-lookup"><span data-stu-id="452a2-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="452a2-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="452a2-131">**reportableIdentifier**</span></span> | <span data-ttu-id="452a2-132">string</span><span class="sxs-lookup"><span data-stu-id="452a2-132">string</span></span> | <span data-ttu-id="452a2-133">このエラーのエントリの識別子です。</span><span class="sxs-lookup"><span data-stu-id="452a2-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="452a2-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="452a2-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
