---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066864"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="fb1ff-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb1ff-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="fb1ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb1ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb1ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb1ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb1ff-106">CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="fb1ff-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="fb1ff-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="fb1ff-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fb1ff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb1ff-108">Properties</span></span>

| <span data-ttu-id="fb1ff-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb1ff-109">Property</span></span> | <span data-ttu-id="fb1ff-110">型</span><span class="sxs-lookup"><span data-stu-id="fb1ff-110">Type</span></span> | <span data-ttu-id="fb1ff-111">説明</span><span class="sxs-lookup"><span data-stu-id="fb1ff-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fb1ff-112">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="fb1ff-112">**customizations**</span></span> | [<span data-ttu-id="fb1ff-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="fb1ff-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="fb1ff-114">同期プロファイルを適用するオプションのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="fb1ff-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb1ff-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb1ff-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
