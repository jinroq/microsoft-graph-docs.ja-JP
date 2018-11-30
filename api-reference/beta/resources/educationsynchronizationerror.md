---
title: educationSynchronizationError リソースの種類
description: 学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。
ms.openlocfilehash: 91a633ab4056e8e86854a0e2d45ae13e22da19a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067101"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="f6606-103">educationSynchronizationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6606-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="f6606-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6606-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6606-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6606-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6606-106">学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。</span><span class="sxs-lookup"><span data-stu-id="f6606-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="f6606-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6606-107">Methods</span></span>

| <span data-ttu-id="f6606-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6606-108">Method</span></span> | <span data-ttu-id="f6606-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f6606-109">Return Type</span></span> | <span data-ttu-id="f6606-110">説明</span><span class="sxs-lookup"><span data-stu-id="f6606-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="f6606-111">同期エラーが発生をします。</span><span class="sxs-lookup"><span data-stu-id="f6606-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="f6606-112">**educationSynchronizationError**コレクション</span><span class="sxs-lookup"><span data-stu-id="f6606-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="f6606-113">プロファイルに関連付けられている同期エラーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="f6606-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="f6606-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6606-114">Properties</span></span>

| <span data-ttu-id="f6606-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6606-115">Property</span></span> | <span data-ttu-id="f6606-116">型</span><span class="sxs-lookup"><span data-stu-id="f6606-116">Type</span></span> | <span data-ttu-id="f6606-117">説明</span><span class="sxs-lookup"><span data-stu-id="f6606-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f6606-118">**示した**</span><span class="sxs-lookup"><span data-stu-id="f6606-118">**entryType**</span></span> | <span data-ttu-id="f6606-119">文字列</span><span class="sxs-lookup"><span data-stu-id="f6606-119">string</span></span> |  <span data-ttu-id="f6606-120">(学校、セクション、学生、教師) は、同期エンティティを表します。</span><span class="sxs-lookup"><span data-stu-id="f6606-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="f6606-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="f6606-121">**errorCode**</span></span> | <span data-ttu-id="f6606-122">文字列</span><span class="sxs-lookup"><span data-stu-id="f6606-122">string</span></span> |  <span data-ttu-id="f6606-123">このエラーのエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="f6606-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="f6606-124">**エラー メッセージ**</span><span class="sxs-lookup"><span data-stu-id="f6606-124">**errorMessage**</span></span> | <span data-ttu-id="f6606-125">文字列</span><span class="sxs-lookup"><span data-stu-id="f6606-125">string</span></span> |  <span data-ttu-id="f6606-126">エラーの説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6606-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="f6606-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="f6606-127">**joiningValue**</span></span> | <span data-ttu-id="f6606-128">文字列</span><span class="sxs-lookup"><span data-stu-id="f6606-128">string</span></span> |  <span data-ttu-id="f6606-129">エントリの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6606-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="f6606-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f6606-130">**recordedDateTime**</span></span> | <span data-ttu-id="f6606-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6606-131">DateTimeOffset</span></span> | <span data-ttu-id="f6606-132">このエラーの発生時刻。</span><span class="sxs-lookup"><span data-stu-id="f6606-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="f6606-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="f6606-133">**reportableIdentifier**</span></span> | <span data-ttu-id="f6606-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f6606-134">string</span></span> | <span data-ttu-id="f6606-135">このエラーのエントリの識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6606-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="f6606-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6606-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
