---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
ms.openlocfilehash: cf685e0619c5600340df68ba86ecaef11a8a435d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066861"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="8613d-105">educationFileSynchronizationVerificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8613d-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="8613d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8613d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8613d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8613d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8613d-108">CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="8613d-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="8613d-109">リソースの検証エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8613d-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="8613d-110">ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8613d-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="8613d-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8613d-111">Properties</span></span>

| <span data-ttu-id="8613d-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8613d-112">Property</span></span> | <span data-ttu-id="8613d-113">型</span><span class="sxs-lookup"><span data-stu-id="8613d-113">Type</span></span> | <span data-ttu-id="8613d-114">説明</span><span class="sxs-lookup"><span data-stu-id="8613d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8613d-115">**type**</span><span class="sxs-lookup"><span data-stu-id="8613d-115">**type**</span></span> | <span data-ttu-id="8613d-116">string</span><span class="sxs-lookup"><span data-stu-id="8613d-116">string</span></span> | <span data-ttu-id="8613d-117">メッセージの種類です。</span><span class="sxs-lookup"><span data-stu-id="8613d-117">Type of the message.</span></span> <span data-ttu-id="8613d-118">可能な値は、`error`、`warning`、`information` です。</span><span class="sxs-lookup"><span data-stu-id="8613d-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="8613d-119">filename</span><span class="sxs-lookup"><span data-stu-id="8613d-119">**filename**</span></span> | <span data-ttu-id="8613d-120">文字列</span><span class="sxs-lookup"><span data-stu-id="8613d-120">string</span></span> | <span data-ttu-id="8613d-121">エラーを含むソース ファイルです。</span><span class="sxs-lookup"><span data-stu-id="8613d-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="8613d-122">**description**</span><span class="sxs-lookup"><span data-stu-id="8613d-122">**description**</span></span> | <span data-ttu-id="8613d-123">文字列</span><span class="sxs-lookup"><span data-stu-id="8613d-123">string</span></span> | <span data-ttu-id="8613d-124">メッセージの種類に関する詳細な情報。</span><span class="sxs-lookup"><span data-stu-id="8613d-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8613d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8613d-125">JSON representation</span></span>

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