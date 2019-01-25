---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529895"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="d032b-105">educationFileSynchronizationVerificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d032b-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d032b-106">CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="d032b-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="d032b-107">リソースの検証エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d032b-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="d032b-108">ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d032b-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="d032b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d032b-109">Properties</span></span>

| <span data-ttu-id="d032b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d032b-110">Property</span></span> | <span data-ttu-id="d032b-111">型</span><span class="sxs-lookup"><span data-stu-id="d032b-111">Type</span></span> | <span data-ttu-id="d032b-112">説明</span><span class="sxs-lookup"><span data-stu-id="d032b-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d032b-113">**type**</span><span class="sxs-lookup"><span data-stu-id="d032b-113">**type**</span></span> | <span data-ttu-id="d032b-114">string</span><span class="sxs-lookup"><span data-stu-id="d032b-114">string</span></span> | <span data-ttu-id="d032b-115">メッセージの種類です。</span><span class="sxs-lookup"><span data-stu-id="d032b-115">Type of the message.</span></span> <span data-ttu-id="d032b-116">可能な値は、`error`、`warning`、`information` です。</span><span class="sxs-lookup"><span data-stu-id="d032b-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="d032b-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="d032b-117">**filename**</span></span> | <span data-ttu-id="d032b-118">string</span><span class="sxs-lookup"><span data-stu-id="d032b-118">string</span></span> | <span data-ttu-id="d032b-119">エラーを含むソース ファイルです。</span><span class="sxs-lookup"><span data-stu-id="d032b-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="d032b-120">**description**</span><span class="sxs-lookup"><span data-stu-id="d032b-120">**description**</span></span> | <span data-ttu-id="d032b-121">string</span><span class="sxs-lookup"><span data-stu-id="d032b-121">string</span></span> | <span data-ttu-id="d032b-122">メッセージの種類に関する詳細な情報。</span><span class="sxs-lookup"><span data-stu-id="d032b-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d032b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d032b-123">JSON representation</span></span>

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
