---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845515"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="7b9b0-105">educationFileSynchronizationVerificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b9b0-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="7b9b0-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b9b0-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b9b0-108">CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="7b9b0-109">リソースの検証エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="7b9b0-110">ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="7b9b0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b9b0-111">Properties</span></span>

| <span data-ttu-id="7b9b0-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b9b0-112">Property</span></span> | <span data-ttu-id="7b9b0-113">種類</span><span class="sxs-lookup"><span data-stu-id="7b9b0-113">Type</span></span> | <span data-ttu-id="7b9b0-114">説明</span><span class="sxs-lookup"><span data-stu-id="7b9b0-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7b9b0-115">**type**</span><span class="sxs-lookup"><span data-stu-id="7b9b0-115">**type**</span></span> | <span data-ttu-id="7b9b0-116">string</span><span class="sxs-lookup"><span data-stu-id="7b9b0-116">string</span></span> | <span data-ttu-id="7b9b0-117">メッセージの種類です。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-117">Type of the message.</span></span> <span data-ttu-id="7b9b0-118">可能な値は、`error`、`warning`、`information` です。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="7b9b0-119">**filename**</span><span class="sxs-lookup"><span data-stu-id="7b9b0-119">**filename**</span></span> | <span data-ttu-id="7b9b0-120">文字列</span><span class="sxs-lookup"><span data-stu-id="7b9b0-120">string</span></span> | <span data-ttu-id="7b9b0-121">エラーを含むソース ファイルです。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="7b9b0-122">**description**</span><span class="sxs-lookup"><span data-stu-id="7b9b0-122">**description**</span></span> | <span data-ttu-id="7b9b0-123">文字列</span><span class="sxs-lookup"><span data-stu-id="7b9b0-123">string</span></span> | <span data-ttu-id="7b9b0-124">メッセージの種類に関する詳細な情報。</span><span class="sxs-lookup"><span data-stu-id="7b9b0-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b9b0-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b9b0-125">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
