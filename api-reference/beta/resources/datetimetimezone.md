---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057044"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="f06f1-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f06f1-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f06f1-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="f06f1-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="f06f1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f06f1-105">Properties</span></span>
| <span data-ttu-id="f06f1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f06f1-106">Property</span></span>     | <span data-ttu-id="f06f1-107">種類</span><span class="sxs-lookup"><span data-stu-id="f06f1-107">Type</span></span>   |<span data-ttu-id="f06f1-108">説明</span><span class="sxs-lookup"><span data-stu-id="f06f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f06f1-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="f06f1-109">dateTime</span></span>|<span data-ttu-id="f06f1-110">String</span><span class="sxs-lookup"><span data-stu-id="f06f1-110">String</span></span>|<span data-ttu-id="f06f1-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`)。</span><span class="sxs-lookup"><span data-stu-id="f06f1-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="f06f1-112">たとえば、"2019-04-16t09:00:00" とします。</span><span class="sxs-lookup"><span data-stu-id="f06f1-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="f06f1-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="f06f1-113">timeZone</span></span>|<span data-ttu-id="f06f1-114">String
</span><span class="sxs-lookup"><span data-stu-id="f06f1-114">String</span></span>|<span data-ttu-id="f06f1-115">次に示すようなタイムゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="f06f1-115">A time zone name as described below.</span></span>|

<span data-ttu-id="f06f1-116">**timeZone**プロパティは、Windows でサポートされている任意のタイムゾーン、および次のタイムゾーン名に設定できます。</span><span class="sxs-lookup"><span data-stu-id="f06f1-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="f06f1-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="f06f1-117">Etc/GMT+12</span></span>

<span data-ttu-id="f06f1-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="f06f1-118">Etc/GMT+11</span></span>

<span data-ttu-id="f06f1-119">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="f06f1-119">Pacific/Honolulu</span></span>

<span data-ttu-id="f06f1-120">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="f06f1-120">America/Anchorage</span></span>

<span data-ttu-id="f06f1-121">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="f06f1-121">America/Santa_Isabel</span></span>

<span data-ttu-id="f06f1-122">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="f06f1-122">America/Los_Angeles</span></span>

<span data-ttu-id="f06f1-123">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="f06f1-123">America/Phoenix</span></span>

<span data-ttu-id="f06f1-124">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="f06f1-124">America/Chihuahua</span></span>

<span data-ttu-id="f06f1-125">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="f06f1-125">America/Denver</span></span>

<span data-ttu-id="f06f1-126">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="f06f1-126">America/Guatemala</span></span>

<span data-ttu-id="f06f1-127">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="f06f1-127">America/Chicago</span></span>

<span data-ttu-id="f06f1-128">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="f06f1-128">America/Mexico_City</span></span>

<span data-ttu-id="f06f1-129">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="f06f1-129">America/Regina</span></span>

<span data-ttu-id="f06f1-130">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="f06f1-130">America/Bogota</span></span>

<span data-ttu-id="f06f1-131">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="f06f1-131">America/New_York</span></span>

<span data-ttu-id="f06f1-132">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="f06f1-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="f06f1-133">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="f06f1-133">America/Caracas</span></span>

<span data-ttu-id="f06f1-134">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="f06f1-134">America/Asuncion</span></span>

<span data-ttu-id="f06f1-135">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="f06f1-135">America/Halifax</span></span>

<span data-ttu-id="f06f1-136">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="f06f1-136">America/Cuiaba</span></span>

<span data-ttu-id="f06f1-137">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="f06f1-137">America/La_Paz</span></span>

<span data-ttu-id="f06f1-138">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="f06f1-138">America/Santiago</span></span>

<span data-ttu-id="f06f1-139">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="f06f1-139">America/St_Johns</span></span>

<span data-ttu-id="f06f1-140">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="f06f1-140">America/Sao_Paulo</span></span>

<span data-ttu-id="f06f1-141">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="f06f1-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="f06f1-142">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="f06f1-142">America/Cayenne</span></span>

<span data-ttu-id="f06f1-143">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="f06f1-143">America/Godthab</span></span>

<span data-ttu-id="f06f1-144">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="f06f1-144">America/Montevideo</span></span>

<span data-ttu-id="f06f1-145">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="f06f1-145">America/Bahia</span></span>

<span data-ttu-id="f06f1-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="f06f1-146">Etc/GMT+2</span></span>

<span data-ttu-id="f06f1-147">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="f06f1-147">Atlantic/Azores</span></span>

<span data-ttu-id="f06f1-148">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="f06f1-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="f06f1-149">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="f06f1-149">Africa/Casablanca</span></span>

<span data-ttu-id="f06f1-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="f06f1-150">Etc/GMT</span></span>

<span data-ttu-id="f06f1-151">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="f06f1-151">Europe/London</span></span>

<span data-ttu-id="f06f1-152">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="f06f1-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="f06f1-153">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="f06f1-153">Europe/Berlin</span></span>

<span data-ttu-id="f06f1-154">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="f06f1-154">Europe/Budapest</span></span>

<span data-ttu-id="f06f1-155">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="f06f1-155">Europe/Paris</span></span>

<span data-ttu-id="f06f1-156">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="f06f1-156">Europe/Warsaw</span></span>

<span data-ttu-id="f06f1-157">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="f06f1-157">Africa/Lagos</span></span>

<span data-ttu-id="f06f1-158">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="f06f1-158">Africa/Windhoek</span></span>

<span data-ttu-id="f06f1-159">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="f06f1-159">Europe/Bucharest</span></span>

<span data-ttu-id="f06f1-160">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="f06f1-160">Asia/Beirut</span></span>

<span data-ttu-id="f06f1-161">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="f06f1-161">Africa/Cairo</span></span>

<span data-ttu-id="f06f1-162">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="f06f1-162">Asia/Damascus</span></span>

<span data-ttu-id="f06f1-163">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="f06f1-163">Africa/Johannesburg</span></span>

<span data-ttu-id="f06f1-164">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="f06f1-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="f06f1-165">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="f06f1-165">Europe/Istanbul</span></span>

<span data-ttu-id="f06f1-166">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="f06f1-166">Asia/Jerusalem</span></span>

<span data-ttu-id="f06f1-167">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="f06f1-167">Asia/Amman</span></span>

<span data-ttu-id="f06f1-168">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="f06f1-168">Asia/Baghdad</span></span>

<span data-ttu-id="f06f1-169">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="f06f1-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="f06f1-170">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="f06f1-170">Asia/Riyadh</span></span>

<span data-ttu-id="f06f1-171">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="f06f1-171">Africa/Nairobi</span></span>

<span data-ttu-id="f06f1-172">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="f06f1-172">Asia/Tehran</span></span>

<span data-ttu-id="f06f1-173">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="f06f1-173">Asia/Dubai</span></span>

<span data-ttu-id="f06f1-174">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="f06f1-174">Asia/Baku</span></span>

<span data-ttu-id="f06f1-175">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="f06f1-175">Europe/Moscow</span></span>

<span data-ttu-id="f06f1-176">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="f06f1-176">Indian/Mauritius</span></span>

<span data-ttu-id="f06f1-177">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="f06f1-177">Asia/Tbilisi</span></span>

<span data-ttu-id="f06f1-178">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="f06f1-178">Asia/Yerevan</span></span>

<span data-ttu-id="f06f1-179">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="f06f1-179">Asia/Kabul</span></span>

<span data-ttu-id="f06f1-180">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="f06f1-180">Asia/Karachi</span></span>

<span data-ttu-id="f06f1-181">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="f06f1-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="f06f1-182">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="f06f1-182">Asia/Kolkata</span></span>

<span data-ttu-id="f06f1-183">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="f06f1-183">Asia/Colombo</span></span>

<span data-ttu-id="f06f1-184">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="f06f1-184">Asia/Kathmandu</span></span>

<span data-ttu-id="f06f1-185">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="f06f1-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="f06f1-186">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="f06f1-186">Asia/Dhaka</span></span>

<span data-ttu-id="f06f1-187">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="f06f1-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="f06f1-188">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="f06f1-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="f06f1-189">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="f06f1-189">Asia/Bangkok</span></span>

<span data-ttu-id="f06f1-190">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="f06f1-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="f06f1-191">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="f06f1-191">Asia/Shanghai</span></span>

<span data-ttu-id="f06f1-192">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="f06f1-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="f06f1-193">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="f06f1-193">Asia/Singapore</span></span>

<span data-ttu-id="f06f1-194">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="f06f1-194">Australia/Perth</span></span>

<span data-ttu-id="f06f1-195">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="f06f1-195">Asia/Taipei</span></span>

<span data-ttu-id="f06f1-196">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="f06f1-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="f06f1-197">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="f06f1-197">Asia/Irkutsk</span></span>

<span data-ttu-id="f06f1-198">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="f06f1-198">Asia/Tokyo</span></span>

<span data-ttu-id="f06f1-199">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="f06f1-199">Asia/Seoul</span></span>

<span data-ttu-id="f06f1-200">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="f06f1-200">Australia/Adelaide</span></span>

<span data-ttu-id="f06f1-201">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="f06f1-201">Australia/Darwin</span></span>

<span data-ttu-id="f06f1-202">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="f06f1-202">Australia/Brisbane</span></span>

<span data-ttu-id="f06f1-203">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="f06f1-203">Australia/Sydney</span></span>

<span data-ttu-id="f06f1-204">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="f06f1-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="f06f1-205">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="f06f1-205">Australia/Hobart</span></span>

<span data-ttu-id="f06f1-206">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="f06f1-206">Asia/Yakutsk</span></span>

<span data-ttu-id="f06f1-207">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="f06f1-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="f06f1-208">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="f06f1-208">Asia/Vladivostok</span></span>

<span data-ttu-id="f06f1-209">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="f06f1-209">Pacific/Auckland</span></span>

<span data-ttu-id="f06f1-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="f06f1-210">Etc/GMT-12</span></span>

<span data-ttu-id="f06f1-211">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="f06f1-211">Pacific/Fiji</span></span>

<span data-ttu-id="f06f1-212">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="f06f1-212">Asia/Magadan</span></span>

<span data-ttu-id="f06f1-213">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="f06f1-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="f06f1-214">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="f06f1-214">Pacific/Apia</span></span>

<span data-ttu-id="f06f1-215">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="f06f1-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="f06f1-216">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f06f1-216">JSON representation</span></span>

<span data-ttu-id="f06f1-217">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f06f1-217">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
