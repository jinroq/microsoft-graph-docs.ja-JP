---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校データプロファイルの同期を開始する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507132"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="fe544-105">educationFileSynchronizationVerificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe544-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe544-106">CSV ベースの学校データプロファイルの[同期を開始](../api/educationsynchronizationprofile-start.md)する要求に対する応答としてクライアントに返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="fe544-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="fe544-107">リソースには、検証結果のエラーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe544-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="fe544-108">azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe544-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="fe544-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe544-109">Properties</span></span>

| <span data-ttu-id="fe544-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe544-110">Property</span></span> | <span data-ttu-id="fe544-111">型</span><span class="sxs-lookup"><span data-stu-id="fe544-111">Type</span></span> | <span data-ttu-id="fe544-112">説明</span><span class="sxs-lookup"><span data-stu-id="fe544-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fe544-113">**type**</span><span class="sxs-lookup"><span data-stu-id="fe544-113">**type**</span></span> | <span data-ttu-id="fe544-114">string</span><span class="sxs-lookup"><span data-stu-id="fe544-114">string</span></span> | <span data-ttu-id="fe544-115">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="fe544-115">Type of the message.</span></span> <span data-ttu-id="fe544-116">使用可能な値は、`error`、`warning`、`information` です。</span><span class="sxs-lookup"><span data-stu-id="fe544-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="fe544-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="fe544-117">**filename**</span></span> | <span data-ttu-id="fe544-118">string</span><span class="sxs-lookup"><span data-stu-id="fe544-118">string</span></span> | <span data-ttu-id="fe544-119">エラーを含むソースファイル。</span><span class="sxs-lookup"><span data-stu-id="fe544-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="fe544-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe544-120">**description**</span></span> | <span data-ttu-id="fe544-121">string</span><span class="sxs-lookup"><span data-stu-id="fe544-121">string</span></span> | <span data-ttu-id="fe544-122">メッセージの種類に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="fe544-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe544-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe544-123">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
