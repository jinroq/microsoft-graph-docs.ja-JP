---
title: educationPowerSchoolDataProvider リソース
description: PowerSchool は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510464"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="6266d-103">educationPowerSchoolDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="6266d-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6266d-104">[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="6266d-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="6266d-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="6266d-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6266d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6266d-106">Properties</span></span>

| <span data-ttu-id="6266d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6266d-107">Property</span></span> | <span data-ttu-id="6266d-108">型</span><span class="sxs-lookup"><span data-stu-id="6266d-108">Type</span></span> | <span data-ttu-id="6266d-109">説明</span><span class="sxs-lookup"><span data-stu-id="6266d-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6266d-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="6266d-110">**connectionUrl**</span></span> | <span data-ttu-id="6266d-111">String</span><span class="sxs-lookup"><span data-stu-id="6266d-111">String</span></span> | <span data-ttu-id="6266d-112">PowerSchool のインスタンスへの接続 URL です。</span><span class="sxs-lookup"><span data-stu-id="6266d-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="6266d-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="6266d-113">**clientId**</span></span> | <span data-ttu-id="6266d-114">String</span><span class="sxs-lookup"><span data-stu-id="6266d-114">String</span></span> |  <span data-ttu-id="6266d-115">クライアント ID は、PowerSchool に接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="6266d-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="6266d-116">client_secret</span><span class="sxs-lookup"><span data-stu-id="6266d-116">**clientSecret**</span></span> | <span data-ttu-id="6266d-117">String</span><span class="sxs-lookup"><span data-stu-id="6266d-117">String</span></span> |  <span data-ttu-id="6266d-118">PowerSchool のインスタンスへの接続を認証するためにクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="6266d-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="6266d-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="6266d-119">**schoolsIds**</span></span> | <span data-ttu-id="6266d-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6266d-120">String collection</span></span> |  <span data-ttu-id="6266d-121">学校の同期のリスト。</span><span class="sxs-lookup"><span data-stu-id="6266d-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="6266d-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="6266d-122">**schoolYear**</span></span> | <span data-ttu-id="6266d-123">String</span><span class="sxs-lookup"><span data-stu-id="6266d-123">String</span></span> |  <span data-ttu-id="6266d-124">同期する学校の年です。</span><span class="sxs-lookup"><span data-stu-id="6266d-124">The school year to sync.</span></span> |
| <span data-ttu-id="6266d-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="6266d-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="6266d-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="6266d-126">Boolean</span></span> |  <span data-ttu-id="6266d-127">ソースが 1 つの学生または教師の複数の識別子を持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6266d-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="6266d-128">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="6266d-128">**customizations**</span></span> | [<span data-ttu-id="6266d-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="6266d-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="6266d-130">同期プロファイルを適用するオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="6266d-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6266d-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6266d-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
