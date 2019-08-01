---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e265e6de20491e44ba7756ffd02f4dc4d09d0b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029541"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="5eb45-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5eb45-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="5eb45-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="5eb45-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="5eb45-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5eb45-105">Properties</span></span>
| <span data-ttu-id="5eb45-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5eb45-106">Property</span></span>     | <span data-ttu-id="5eb45-107">型</span><span class="sxs-lookup"><span data-stu-id="5eb45-107">Type</span></span>   |<span data-ttu-id="5eb45-108">説明</span><span class="sxs-lookup"><span data-stu-id="5eb45-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5eb45-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="5eb45-109">dateTime</span></span>|<span data-ttu-id="5eb45-110">String</span><span class="sxs-lookup"><span data-stu-id="5eb45-110">String</span></span>|<span data-ttu-id="5eb45-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`、例 `2017-08-29T04:00:00.0000000`)。</span><span class="sxs-lookup"><span data-stu-id="5eb45-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="5eb45-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="5eb45-112">timeZone</span></span>|<span data-ttu-id="5eb45-113">String</span><span class="sxs-lookup"><span data-stu-id="5eb45-113">String</span></span>|<span data-ttu-id="5eb45-114">"太平洋標準時" などのタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="5eb45-114">A string representing a specific time zone for the response, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="5eb45-115">指定可能な値の詳細については、下記をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5eb45-115">See below for information about the possible values.</span></span>|

<span data-ttu-id="5eb45-116">通常、**timeZone** プロパティは、追加の[カレンダー API でサポートされているタイム ゾーン](#additional-time-zones)と同様に、[Windows で現在サポートされている任意のタイム ゾーンに設定](https://docs.microsoft.com/ja-JP/windows-hardware/manufacture/desktop/default-time-zones) _できます_。</span><span class="sxs-lookup"><span data-stu-id="5eb45-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="5eb45-117">メソッド (イベントの[作成](../api/user-post-events.md) または [更新](../api/event-update.md)など)と併用して**dateTimeTimeZone**を使用する場合は、実際にサポートされているタイム ゾーンをメモしますが、それはより小さいサブセットになります。</span><span class="sxs-lookup"><span data-stu-id="5eb45-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="5eb45-118">追加のタイム ゾーン</span><span class="sxs-lookup"><span data-stu-id="5eb45-118">Additional time zones</span></span>

<span data-ttu-id="5eb45-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="5eb45-119">Etc/GMT+12</span></span>

<span data-ttu-id="5eb45-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="5eb45-120">Etc/GMT+11</span></span>

<span data-ttu-id="5eb45-121">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="5eb45-121">Pacific/Honolulu</span></span>

<span data-ttu-id="5eb45-122">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="5eb45-122">America/Anchorage</span></span>

<span data-ttu-id="5eb45-123">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="5eb45-123">America/Santa_Isabel</span></span>

<span data-ttu-id="5eb45-124">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="5eb45-124">America/Los_Angeles</span></span>

<span data-ttu-id="5eb45-125">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="5eb45-125">America/Phoenix</span></span>

<span data-ttu-id="5eb45-126">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="5eb45-126">America/Chihuahua</span></span>

<span data-ttu-id="5eb45-127">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="5eb45-127">America/Denver</span></span>

<span data-ttu-id="5eb45-128">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="5eb45-128">America/Guatemala</span></span>

<span data-ttu-id="5eb45-129">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="5eb45-129">America/Chicago</span></span>

<span data-ttu-id="5eb45-130">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="5eb45-130">America/Mexico_City</span></span>

<span data-ttu-id="5eb45-131">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="5eb45-131">America/Regina</span></span>

<span data-ttu-id="5eb45-132">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="5eb45-132">America/Bogota</span></span>

<span data-ttu-id="5eb45-133">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="5eb45-133">America/New_York</span></span>

<span data-ttu-id="5eb45-134">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="5eb45-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="5eb45-135">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="5eb45-135">America/Caracas</span></span>

<span data-ttu-id="5eb45-136">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="5eb45-136">America/Asuncion</span></span>

<span data-ttu-id="5eb45-137">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="5eb45-137">America/Halifax</span></span>

<span data-ttu-id="5eb45-138">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="5eb45-138">America/Cuiaba</span></span>

<span data-ttu-id="5eb45-139">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="5eb45-139">America/La_Paz</span></span>

<span data-ttu-id="5eb45-140">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="5eb45-140">America/Santiago</span></span>

<span data-ttu-id="5eb45-141">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="5eb45-141">America/St_Johns</span></span>

<span data-ttu-id="5eb45-142">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="5eb45-142">America/Sao_Paulo</span></span>

<span data-ttu-id="5eb45-143">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="5eb45-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="5eb45-144">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="5eb45-144">America/Cayenne</span></span>

<span data-ttu-id="5eb45-145">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="5eb45-145">America/Godthab</span></span>

<span data-ttu-id="5eb45-146">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="5eb45-146">America/Montevideo</span></span>

<span data-ttu-id="5eb45-147">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="5eb45-147">America/Bahia</span></span>

<span data-ttu-id="5eb45-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="5eb45-148">Etc/GMT+2</span></span>

<span data-ttu-id="5eb45-149">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="5eb45-149">Atlantic/Azores</span></span>

<span data-ttu-id="5eb45-150">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="5eb45-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="5eb45-151">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="5eb45-151">Africa/Casablanca</span></span>

<span data-ttu-id="5eb45-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="5eb45-152">Etc/GMT</span></span>

<span data-ttu-id="5eb45-153">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="5eb45-153">Europe/London</span></span>

<span data-ttu-id="5eb45-154">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="5eb45-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="5eb45-155">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="5eb45-155">Europe/Berlin</span></span>

<span data-ttu-id="5eb45-156">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="5eb45-156">Europe/Budapest</span></span>

<span data-ttu-id="5eb45-157">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="5eb45-157">Europe/Paris</span></span>

<span data-ttu-id="5eb45-158">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="5eb45-158">Europe/Warsaw</span></span>

<span data-ttu-id="5eb45-159">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="5eb45-159">Africa/Lagos</span></span>

<span data-ttu-id="5eb45-160">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="5eb45-160">Africa/Windhoek</span></span>

<span data-ttu-id="5eb45-161">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="5eb45-161">Europe/Bucharest</span></span>

<span data-ttu-id="5eb45-162">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="5eb45-162">Asia/Beirut</span></span>

<span data-ttu-id="5eb45-163">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="5eb45-163">Africa/Cairo</span></span>

<span data-ttu-id="5eb45-164">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="5eb45-164">Asia/Damascus</span></span>

<span data-ttu-id="5eb45-165">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="5eb45-165">Africa/Johannesburg</span></span>

<span data-ttu-id="5eb45-166">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="5eb45-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="5eb45-167">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="5eb45-167">Europe/Istanbul</span></span>

<span data-ttu-id="5eb45-168">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="5eb45-168">Asia/Jerusalem</span></span>

<span data-ttu-id="5eb45-169">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="5eb45-169">Asia/Amman</span></span>

<span data-ttu-id="5eb45-170">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="5eb45-170">Asia/Baghdad</span></span>

<span data-ttu-id="5eb45-171">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="5eb45-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="5eb45-172">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="5eb45-172">Asia/Riyadh</span></span>

<span data-ttu-id="5eb45-173">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="5eb45-173">Africa/Nairobi</span></span>

<span data-ttu-id="5eb45-174">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="5eb45-174">Asia/Tehran</span></span>

<span data-ttu-id="5eb45-175">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="5eb45-175">Asia/Dubai</span></span>

<span data-ttu-id="5eb45-176">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="5eb45-176">Asia/Baku</span></span>

<span data-ttu-id="5eb45-177">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="5eb45-177">Europe/Moscow</span></span>

<span data-ttu-id="5eb45-178">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="5eb45-178">Indian/Mauritius</span></span>

<span data-ttu-id="5eb45-179">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="5eb45-179">Asia/Tbilisi</span></span>

<span data-ttu-id="5eb45-180">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="5eb45-180">Asia/Yerevan</span></span>

<span data-ttu-id="5eb45-181">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="5eb45-181">Asia/Kabul</span></span>

<span data-ttu-id="5eb45-182">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="5eb45-182">Asia/Karachi</span></span>

<span data-ttu-id="5eb45-183">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="5eb45-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="5eb45-184">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="5eb45-184">Asia/Kolkata</span></span>

<span data-ttu-id="5eb45-185">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="5eb45-185">Asia/Colombo</span></span>

<span data-ttu-id="5eb45-186">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="5eb45-186">Asia/Kathmandu</span></span>

<span data-ttu-id="5eb45-187">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="5eb45-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="5eb45-188">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="5eb45-188">Asia/Dhaka</span></span>

<span data-ttu-id="5eb45-189">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="5eb45-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="5eb45-190">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="5eb45-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="5eb45-191">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="5eb45-191">Asia/Bangkok</span></span>

<span data-ttu-id="5eb45-192">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="5eb45-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="5eb45-193">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="5eb45-193">Asia/Shanghai</span></span>

<span data-ttu-id="5eb45-194">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="5eb45-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="5eb45-195">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="5eb45-195">Asia/Singapore</span></span>

<span data-ttu-id="5eb45-196">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="5eb45-196">Australia/Perth</span></span>

<span data-ttu-id="5eb45-197">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="5eb45-197">Asia/Taipei</span></span>

<span data-ttu-id="5eb45-198">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="5eb45-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="5eb45-199">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="5eb45-199">Asia/Irkutsk</span></span>

<span data-ttu-id="5eb45-200">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="5eb45-200">Asia/Tokyo</span></span>

<span data-ttu-id="5eb45-201">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="5eb45-201">Asia/Seoul</span></span>

<span data-ttu-id="5eb45-202">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="5eb45-202">Australia/Adelaide</span></span>

<span data-ttu-id="5eb45-203">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="5eb45-203">Australia/Darwin</span></span>

<span data-ttu-id="5eb45-204">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="5eb45-204">Australia/Brisbane</span></span>

<span data-ttu-id="5eb45-205">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="5eb45-205">Australia/Sydney</span></span>

<span data-ttu-id="5eb45-206">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="5eb45-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="5eb45-207">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="5eb45-207">Australia/Hobart</span></span>

<span data-ttu-id="5eb45-208">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="5eb45-208">Asia/Yakutsk</span></span>

<span data-ttu-id="5eb45-209">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="5eb45-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="5eb45-210">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="5eb45-210">Asia/Vladivostok</span></span>

<span data-ttu-id="5eb45-211">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="5eb45-211">Pacific/Auckland</span></span>

<span data-ttu-id="5eb45-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="5eb45-212">Etc/GMT-12</span></span>

<span data-ttu-id="5eb45-213">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="5eb45-213">Pacific/Fiji</span></span>

<span data-ttu-id="5eb45-214">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="5eb45-214">Asia/Magadan</span></span>

<span data-ttu-id="5eb45-215">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="5eb45-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="5eb45-216">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="5eb45-216">Pacific/Apia</span></span>

<span data-ttu-id="5eb45-217">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="5eb45-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="5eb45-218">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5eb45-218">JSON representation</span></span>

<span data-ttu-id="5eb45-219">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5eb45-219">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
