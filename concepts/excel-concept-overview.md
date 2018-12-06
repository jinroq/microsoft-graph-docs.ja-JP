---
title: Excel のブックとグラフの API の概要
description: Excel は、必要不可欠な生産性向上ツールです。 あらゆる業界と職務のユーザーが、あらゆる種類のデータを保存、追跡、操作するためのツールとして採用しています。 簡単なタスク追跡やデータ管理から複雑な計算や本格的なレポートに至るまで、あらゆる作業に使用されます。 Microsoft Graph で Excel REST API を使用して、データ、計算、レポート、およびダッシュボードの値を拡張できます。
ms.openlocfilehash: 4d433b4b84bab2fc6a75cf8d0020d715a030683b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092547"
---
# <a name="excel-workbooks-and-charts-api-overview"></a><span data-ttu-id="f12bf-106">Excel のブックとグラフの API の概要</span><span class="sxs-lookup"><span data-stu-id="f12bf-106">Excel workbooks and charts API overview</span></span>

<span data-ttu-id="f12bf-107">Excel は、必要不可欠な生産性向上ツールです。</span><span class="sxs-lookup"><span data-stu-id="f12bf-107">Excel is an indispensable productivity tool.</span></span> <span data-ttu-id="f12bf-108">あらゆる業界と職務のユーザーが、あらゆる種類のデータを保存、追跡、操作するためのツールとして採用しています。</span><span class="sxs-lookup"><span data-stu-id="f12bf-108">Users across all industries and job functions embrace it as a tool for storing, tracking, and manipulating all kinds of data.</span></span> <span data-ttu-id="f12bf-109">簡単なタスク追跡やデータ管理から複雑な計算や本格的なレポートに至るまで、あらゆる作業に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-109">It's used for everything from simple task tracking and data management, to complex calculations and professional reporting.</span></span> <span data-ttu-id="f12bf-110">Microsoft Graph で Excel REST API を使用して、データ、計算、レポート、およびダッシュボードの値を拡張できます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-110">You can use the Excel REST API in Microsoft Graph to extend the value of your data, calculations, reporting, and dashboards.</span></span>

## <a name="why-integrate-with-excel"></a><span data-ttu-id="f12bf-111">Excel と統合する理由</span><span class="sxs-lookup"><span data-stu-id="f12bf-111">Why integrate with Excel?</span></span>

<span data-ttu-id="f12bf-112">Microsoft Graph を使用すると、OneDrive、SharePoint、またはその他のサポートされているストレージ プラットフォームに格納されている Excel ブックを、Web アプリケーションやモバイル アプリケーションで読み取ったり変更したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-112">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms.</span></span>

### <a name="perform-calculations"></a><span data-ttu-id="f12bf-113">計算の実行</span><span class="sxs-lookup"><span data-stu-id="f12bf-113">Perform calculations</span></span>

<span data-ttu-id="f12bf-114">ユーザーは、Excel 内で詳細かつ複雑な計算を簡単に実行できる点を非常に気に入っています。</span><span class="sxs-lookup"><span data-stu-id="f12bf-114">Users love the ease with which they can perform deep and complex calculations within Excel.</span></span> <span data-ttu-id="f12bf-115">今では、Excel の強力な計算エンジンにアクセスして瞬時に結果を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-115">You can now access Excel’s powerful calculation engine with instant results.</span></span> <span data-ttu-id="f12bf-116">たとえば、住宅ローン計算アプリで元金、金利、支払回数を含む簡単な API 呼び出しを行うことにより、Excel の PMT 関数を利用できます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-116">For example, a mortgage calculator can take advantage of the PMT function from Excel by making a simple API call that includes principal, rate and number of payments.</span></span> <span data-ttu-id="f12bf-117">Excel が難しい作業をすべて行い、瞬時に毎月の返済額を返します。</span><span class="sxs-lookup"><span data-stu-id="f12bf-117">Excel does all the difficult work and returns the monthly payment instantly.</span></span> <span data-ttu-id="f12bf-118">現在、300 以上の Excel ワークシート関数が利用可能であり、Excel でサポートされている広範囲の数式に完全にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-118">With more than 300 Excel worksheet functions currently available, you have full access to the breadth of formulas supported by Excel today.</span></span> <span data-ttu-id="f12bf-119">複雑なビジネス モデルを繰り返し再構築する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="f12bf-119">Complex business models don’t need to be rebuilt repeatedly.</span></span> <span data-ttu-id="f12bf-120">開発者は、簡単な API 呼び出しによってこれらの計算を瞬時に実行し、結果を取得するように Excel をプログラミングできます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-120">Developers can program Excel to perform those calculations instantly and retrieve the results with simple API calls.</span></span>

### <a name="generate-reports-and-analyze-results"></a><span data-ttu-id="f12bf-121">レポートの生成と結果の分析</span><span class="sxs-lookup"><span data-stu-id="f12bf-121">Generate reports and analyze results</span></span>

<span data-ttu-id="f12bf-122">Excel は、簡単なデータ テーブルから複雑で本格的なダッシュボードまでをカバーする柔軟なレポートおよび分析ツールです。</span><span class="sxs-lookup"><span data-stu-id="f12bf-122">Excel is a flexible reporting and analysis tool, from simple data tables to complex professional dashboards.</span></span> <span data-ttu-id="f12bf-123">現在では、Excel のすべてのレポート機能への完全なアクセスが提供され、Excel は Office 365 内のオンライン レポート サービスになっています。</span><span class="sxs-lookup"><span data-stu-id="f12bf-123">Today, we give you full access to all of Excel’s reporting features, making Excel an online reporting service within Office 365.</span></span> <span data-ttu-id="f12bf-124">ユーザーが現在作成し、利用しているレポート作成シナリオをカスタム アプリに取り込み、本格的なグラフ作成や大量のデータ分析をインテリジェントに行うことで、Excel がこれらのカスタマイズされたエクスペリエンスにシームレスに融合されることを想像してみてください。</span><span class="sxs-lookup"><span data-stu-id="f12bf-124">Imagine any of the reporting scenarios users create and rely on today pulled into a custom app to create professional charts or analyze large sets of data intelligently, seamlessly blending Excel into those customized experiences.</span></span>

### <a name="store-and-track-data"></a><span data-ttu-id="f12bf-125">データの保存と追跡</span><span class="sxs-lookup"><span data-stu-id="f12bf-125">Store and track data</span></span>

<span data-ttu-id="f12bf-126">Excel は、データを保存して追跡するための優れたツールでもあります。</span><span class="sxs-lookup"><span data-stu-id="f12bf-126">Excel is also a great tool to store and track data.</span></span> <span data-ttu-id="f12bf-127">情報がブックに保存されている場合、そのデータは Office 365 と統合されている任意のアプリで使用できます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-127">If your information is stored in a workbook, that data is available to any app that integrates with Office 365.</span></span> <span data-ttu-id="f12bf-128">そのコンテンツをカスタム ソリューションで読み取り、それらのソリューションのデータ ストレージとして Excel を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-128">Its contents are available to read from custom solutions, and those solutions can use Excel for data storage.</span></span>

><span data-ttu-id="f12bf-129">**注:** Excel の REST API では、Office Open XML ファイル形式のブック (`.xlsx` 拡張子のブック) のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f12bf-129">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks (files with the`.xlsx` extension).</span></span> <span data-ttu-id="f12bf-130">`.xls` 拡張子のブックはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f12bf-130">The `.xls` extension workbooks are not supported.</span></span> 

### <a name="using-the-excel-rest-api"></a><span data-ttu-id="f12bf-131">Excel REST API の使用</span><span class="sxs-lookup"><span data-stu-id="f12bf-131">Using the Excel REST API</span></span>
<span data-ttu-id="f12bf-p107">Microsoft Graph を使用すると、OneDrive、SharePoint、またはその他のサポートされているストレージ プラットフォームに格納されている Excel ブックを、Web アプリケーションやモバイル アプリケーションで読み取ったり変更したりすることができます。`Workbook` (つまり Excel ファイル) リソースには、リレーションシップを介するその他のすべての Excel リソースが含まれています。ファイルの場所を URL で指定すれば、ドライブ API でブックにアクセスできます。例:</span><span class="sxs-lookup"><span data-stu-id="f12bf-p107">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the Drive API by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/ `

<span data-ttu-id="f12bf-136">ブックに対して作成、読み取り、更新、削除 (CRUD) 操作を実行するための標準 REST API を使用して、一連の Excel オブジェクト (テーブル、範囲、グラフなど) にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f12bf-136">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform create, read, update, and delete (CRUD) operations on the workbook.</span></span>

## <a name="api-reference"></a><span data-ttu-id="f12bf-137">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="f12bf-137">API reference</span></span>
<span data-ttu-id="f12bf-138">このサービスの API リファレンスを検索してください。</span><span class="sxs-lookup"><span data-stu-id="f12bf-138">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="f12bf-139">Graph v1.0 Excel API</span><span class="sxs-lookup"><span data-stu-id="f12bf-139">Excel API in Microsoft Graph v1.0</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
- [<span data-ttu-id="f12bf-140">Graph のベータ版の Excel の API</span><span class="sxs-lookup"><span data-stu-id="f12bf-140">Excel API in Microsoft Graph beta</span></span>](/graph/api/resources/excel?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="f12bf-141">次の手順</span><span class="sxs-lookup"><span data-stu-id="f12bf-141">Next steps</span></span>

* [<span data-ttu-id="f12bf-142">Microsoft Graph で Excel のセッションを管理する</span><span class="sxs-lookup"><span data-stu-id="f12bf-142">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="f12bf-143">Microsoft Graph を使用して Excel ブックに書き込む</span><span class="sxs-lookup"><span data-stu-id="f12bf-143">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="f12bf-144">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="f12bf-144">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="f12bf-145">Microsoft Graph により Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="f12bf-145">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="f12bf-146">Microsoft Graph により Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="f12bf-146">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="f12bf-147">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="f12bf-147">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
