---
title: educationSynchronizationError リソースの種類
description: school data profile validation または sync の間に発生したエラーを表します。azure Active Directory (azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542966"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="ef486-103">educationSynchronizationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef486-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef486-104">school data profile validation または sync の間に発生したエラーを表します。azure Active Directory (azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。</span><span class="sxs-lookup"><span data-stu-id="ef486-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="ef486-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef486-105">Methods</span></span>

| <span data-ttu-id="ef486-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef486-106">Method</span></span> | <span data-ttu-id="ef486-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef486-107">Return Type</span></span> | <span data-ttu-id="ef486-108">説明</span><span class="sxs-lookup"><span data-stu-id="ef486-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="ef486-109">同期エラーを取得する</span><span class="sxs-lookup"><span data-stu-id="ef486-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="ef486-110">**educationSynchronizationError**コレクション</span><span class="sxs-lookup"><span data-stu-id="ef486-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="ef486-111">プロファイルに関連付けられている同期エラーのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="ef486-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef486-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef486-112">Properties</span></span>

| <span data-ttu-id="ef486-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef486-113">Property</span></span> | <span data-ttu-id="ef486-114">型</span><span class="sxs-lookup"><span data-stu-id="ef486-114">Type</span></span> | <span data-ttu-id="ef486-115">説明</span><span class="sxs-lookup"><span data-stu-id="ef486-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ef486-116">**entrytype**</span><span class="sxs-lookup"><span data-stu-id="ef486-116">**entryType**</span></span> | <span data-ttu-id="ef486-117">string</span><span class="sxs-lookup"><span data-stu-id="ef486-117">string</span></span> |  <span data-ttu-id="ef486-118">同期エンティティ (school、section、student、教師) を表します。</span><span class="sxs-lookup"><span data-stu-id="ef486-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="ef486-119">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="ef486-119">**errorCode**</span></span> | <span data-ttu-id="ef486-120">string</span><span class="sxs-lookup"><span data-stu-id="ef486-120">string</span></span> |  <span data-ttu-id="ef486-121">このエラーのエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="ef486-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="ef486-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="ef486-122">**errorMessage**</span></span> | <span data-ttu-id="ef486-123">string</span><span class="sxs-lookup"><span data-stu-id="ef486-123">string</span></span> |  <span data-ttu-id="ef486-124">エラーの説明を格納します。</span><span class="sxs-lookup"><span data-stu-id="ef486-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="ef486-125">**joiningvalue**</span><span class="sxs-lookup"><span data-stu-id="ef486-125">**joiningValue**</span></span> | <span data-ttu-id="ef486-126">string</span><span class="sxs-lookup"><span data-stu-id="ef486-126">string</span></span> |  <span data-ttu-id="ef486-127">エントリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ef486-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="ef486-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef486-128">**recordedDateTime**</span></span> | <span data-ttu-id="ef486-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef486-129">DateTimeOffset</span></span> | <span data-ttu-id="ef486-130">このエラーが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="ef486-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="ef486-131">**reportableidentifier**</span><span class="sxs-lookup"><span data-stu-id="ef486-131">**reportableIdentifier**</span></span> | <span data-ttu-id="ef486-132">string</span><span class="sxs-lookup"><span data-stu-id="ef486-132">string</span></span> | <span data-ttu-id="ef486-133">このエラーエントリの識別子。</span><span class="sxs-lookup"><span data-stu-id="ef486-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="ef486-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef486-134">JSON representation</span></span>
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
