---
title: educationSynchronizationError リソースの種類
description: School data profile validation または sync の間に発生したエラーを表します。Azure Active Directory (Azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 11e5be9893c6a50615774e0d2a8e4d51c9576da6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972412"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="7de09-103">educationSynchronizationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7de09-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de09-104">School data profile validation または sync の間に発生したエラーを表します。Azure Active Directory (Azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。</span><span class="sxs-lookup"><span data-stu-id="7de09-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="7de09-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7de09-105">Methods</span></span>

| <span data-ttu-id="7de09-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7de09-106">Method</span></span> | <span data-ttu-id="7de09-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7de09-107">Return Type</span></span> | <span data-ttu-id="7de09-108">説明</span><span class="sxs-lookup"><span data-stu-id="7de09-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="7de09-109">同期エラーを取得する</span><span class="sxs-lookup"><span data-stu-id="7de09-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="7de09-110">**educationSynchronizationError**コレクション</span><span class="sxs-lookup"><span data-stu-id="7de09-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="7de09-111">プロファイルに関連付けられている同期エラーのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="7de09-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="7de09-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de09-112">Properties</span></span>

| <span data-ttu-id="7de09-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de09-113">Property</span></span> | <span data-ttu-id="7de09-114">型</span><span class="sxs-lookup"><span data-stu-id="7de09-114">Type</span></span> | <span data-ttu-id="7de09-115">説明</span><span class="sxs-lookup"><span data-stu-id="7de09-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7de09-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="7de09-116">**entryType**</span></span> | <span data-ttu-id="7de09-117">string</span><span class="sxs-lookup"><span data-stu-id="7de09-117">string</span></span> |  <span data-ttu-id="7de09-118">同期エンティティ (school、section、student、教師) を表します。</span><span class="sxs-lookup"><span data-stu-id="7de09-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="7de09-119">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="7de09-119">**errorCode**</span></span> | <span data-ttu-id="7de09-120">string</span><span class="sxs-lookup"><span data-stu-id="7de09-120">string</span></span> |  <span data-ttu-id="7de09-121">このエラーのエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="7de09-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="7de09-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="7de09-122">**errorMessage**</span></span> | <span data-ttu-id="7de09-123">string</span><span class="sxs-lookup"><span data-stu-id="7de09-123">string</span></span> |  <span data-ttu-id="7de09-124">エラーの説明を格納します。</span><span class="sxs-lookup"><span data-stu-id="7de09-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="7de09-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="7de09-125">**joiningValue**</span></span> | <span data-ttu-id="7de09-126">string</span><span class="sxs-lookup"><span data-stu-id="7de09-126">string</span></span> |  <span data-ttu-id="7de09-127">エントリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7de09-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="7de09-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7de09-128">**recordedDateTime**</span></span> | <span data-ttu-id="7de09-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7de09-129">DateTimeOffset</span></span> | <span data-ttu-id="7de09-130">このエラーが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="7de09-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="7de09-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="7de09-131">**reportableIdentifier**</span></span> | <span data-ttu-id="7de09-132">string</span><span class="sxs-lookup"><span data-stu-id="7de09-132">string</span></span> | <span data-ttu-id="7de09-133">このエラーエントリの識別子。</span><span class="sxs-lookup"><span data-stu-id="7de09-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="7de09-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7de09-134">JSON representation</span></span>
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
