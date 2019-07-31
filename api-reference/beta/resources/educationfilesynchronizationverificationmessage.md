---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校データプロファイルの同期を開始する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 Azure Active Directory (Azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cf462873226ff4238f95ffc4798b6eb662666f3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006410"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="97b37-105">educationFileSynchronizationVerificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97b37-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97b37-106">CSV ベースの学校データプロファイルの[同期を開始](../api/educationsynchronizationprofile-start.md)する要求に対する応答としてクライアントに返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="97b37-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="97b37-107">リソースには、検証結果のエラーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="97b37-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="97b37-108">Azure Active Directory (Azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97b37-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="97b37-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97b37-109">Properties</span></span>

| <span data-ttu-id="97b37-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97b37-110">Property</span></span> | <span data-ttu-id="97b37-111">型</span><span class="sxs-lookup"><span data-stu-id="97b37-111">Type</span></span> | <span data-ttu-id="97b37-112">説明</span><span class="sxs-lookup"><span data-stu-id="97b37-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="97b37-113">**type**</span><span class="sxs-lookup"><span data-stu-id="97b37-113">**type**</span></span> | <span data-ttu-id="97b37-114">string</span><span class="sxs-lookup"><span data-stu-id="97b37-114">string</span></span> | <span data-ttu-id="97b37-115">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="97b37-115">Type of the message.</span></span> <span data-ttu-id="97b37-116">可能な値は、`error`、`warning`、`information` です。</span><span class="sxs-lookup"><span data-stu-id="97b37-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="97b37-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="97b37-117">**filename**</span></span> | <span data-ttu-id="97b37-118">string</span><span class="sxs-lookup"><span data-stu-id="97b37-118">string</span></span> | <span data-ttu-id="97b37-119">エラーを含むソースファイル。</span><span class="sxs-lookup"><span data-stu-id="97b37-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="97b37-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="97b37-120">**description**</span></span> | <span data-ttu-id="97b37-121">string</span><span class="sxs-lookup"><span data-stu-id="97b37-121">string</span></span> | <span data-ttu-id="97b37-122">メッセージの種類に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="97b37-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97b37-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97b37-123">JSON representation</span></span>

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
