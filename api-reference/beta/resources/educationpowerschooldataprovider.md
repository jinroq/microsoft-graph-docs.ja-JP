---
title: educationPowerSchoolDataProvider リソース
description: PowerSchool は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a22c3cf68a4a5b4c12dc4e7105f17eed4fc006f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982758"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="ca879-103">educationPowerSchoolDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="ca879-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="ca879-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca879-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca879-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca879-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca879-106">[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ca879-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="ca879-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="ca879-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca879-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca879-108">Properties</span></span>

| <span data-ttu-id="ca879-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca879-109">Property</span></span> | <span data-ttu-id="ca879-110">型</span><span class="sxs-lookup"><span data-stu-id="ca879-110">Type</span></span> | <span data-ttu-id="ca879-111">説明</span><span class="sxs-lookup"><span data-stu-id="ca879-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ca879-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="ca879-112">**connectionUrl**</span></span> | <span data-ttu-id="ca879-113">String</span><span class="sxs-lookup"><span data-stu-id="ca879-113">String</span></span> | <span data-ttu-id="ca879-114">PowerSchool のインスタンスへの接続 URL です。</span><span class="sxs-lookup"><span data-stu-id="ca879-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="ca879-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="ca879-115">**clientId**</span></span> | <span data-ttu-id="ca879-116">String</span><span class="sxs-lookup"><span data-stu-id="ca879-116">String</span></span> |  <span data-ttu-id="ca879-117">クライアント ID は、PowerSchool に接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ca879-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="ca879-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="ca879-118">**clientSecret**</span></span> | <span data-ttu-id="ca879-119">String</span><span class="sxs-lookup"><span data-stu-id="ca879-119">String</span></span> |  <span data-ttu-id="ca879-120">PowerSchool のインスタンスへの接続を認証するためにクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="ca879-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="ca879-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="ca879-121">**schoolsIds**</span></span> | <span data-ttu-id="ca879-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ca879-122">String collection</span></span> |  <span data-ttu-id="ca879-123">学校の同期のリスト。</span><span class="sxs-lookup"><span data-stu-id="ca879-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="ca879-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="ca879-124">**schoolYear**</span></span> | <span data-ttu-id="ca879-125">String</span><span class="sxs-lookup"><span data-stu-id="ca879-125">String</span></span> |  <span data-ttu-id="ca879-126">同期する学校の年です。</span><span class="sxs-lookup"><span data-stu-id="ca879-126">The school year to sync.</span></span> |
| <span data-ttu-id="ca879-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="ca879-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="ca879-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca879-128">Boolean</span></span> |  <span data-ttu-id="ca879-129">ソースが 1 つの学生または教師の複数の識別子を持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ca879-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="ca879-130">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="ca879-130">**customizations**</span></span> | [<span data-ttu-id="ca879-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="ca879-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="ca879-132">同期プロファイルを適用するオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="ca879-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca879-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca879-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
