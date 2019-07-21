---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5927c10a99b91e0130b8ceb30c33ae1fa19af3dd
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805054"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="7b276-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b276-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="7b276-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="7b276-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="7b276-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b276-105">Properties</span></span>
| <span data-ttu-id="7b276-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b276-106">Property</span></span>     | <span data-ttu-id="7b276-107">型</span><span class="sxs-lookup"><span data-stu-id="7b276-107">Type</span></span>   |<span data-ttu-id="7b276-108">説明</span><span class="sxs-lookup"><span data-stu-id="7b276-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b276-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="7b276-109">dateTime</span></span>|<span data-ttu-id="7b276-110">String</span><span class="sxs-lookup"><span data-stu-id="7b276-110">String</span></span>|<span data-ttu-id="7b276-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`、例 `2017-08-29T04:00:00.0000000`)。</span><span class="sxs-lookup"><span data-stu-id="7b276-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="7b276-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="7b276-112">timeZone</span></span>|<span data-ttu-id="7b276-113">String</span><span class="sxs-lookup"><span data-stu-id="7b276-113">String</span></span>|<span data-ttu-id="7b276-114">"太平洋標準時" などのタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="7b276-114">A string representing a specific time zone for the response, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="7b276-115">指定可能な値の詳細については、下記をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7b276-115">See below for information about the possible values.</span></span>|

<span data-ttu-id="7b276-116">通常、**timeZone** プロパティは、追加の[カレンダー API でサポートされているタイム ゾーン](#additional-time-zones)と同様に、[Windows で現在サポートされている任意のタイム ゾーンに設定](https://docs.microsoft.com/ja-JP/windows-hardware/manufacture/desktop/default-time-zones) _できます_。</span><span class="sxs-lookup"><span data-stu-id="7b276-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="7b276-117">メソッド (イベントの[作成](../api/user-post-events.md) または [更新](../api/event-update.md)など)と併用して**dateTimeTimeZone**を使用する場合は、実際にサポートされているタイム ゾーンをメモしますが、それはより小さいサブセットになります。</span><span class="sxs-lookup"><span data-stu-id="7b276-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="7b276-118">追加のタイム ゾーン</span><span class="sxs-lookup"><span data-stu-id="7b276-118">Additional time zones</span></span>

<span data-ttu-id="7b276-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="7b276-119">Etc/GMT+12</span></span>

<span data-ttu-id="7b276-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="7b276-120">Etc/GMT+11</span></span>

<span data-ttu-id="7b276-121">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="7b276-121">Pacific/Honolulu</span></span>

<span data-ttu-id="7b276-122">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="7b276-122">America/Anchorage</span></span>

<span data-ttu-id="7b276-123">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="7b276-123">America/Santa_Isabel</span></span>

<span data-ttu-id="7b276-124">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="7b276-124">America/Los_Angeles</span></span>

<span data-ttu-id="7b276-125">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="7b276-125">America/Phoenix</span></span>

<span data-ttu-id="7b276-126">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="7b276-126">America/Chihuahua</span></span>

<span data-ttu-id="7b276-127">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="7b276-127">America/Denver</span></span>

<span data-ttu-id="7b276-128">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="7b276-128">America/Guatemala</span></span>

<span data-ttu-id="7b276-129">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="7b276-129">America/Chicago</span></span>

<span data-ttu-id="7b276-130">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="7b276-130">America/Mexico_City</span></span>

<span data-ttu-id="7b276-131">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="7b276-131">America/Regina</span></span>

<span data-ttu-id="7b276-132">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="7b276-132">America/Bogota</span></span>

<span data-ttu-id="7b276-133">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="7b276-133">America/New_York</span></span>

<span data-ttu-id="7b276-134">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="7b276-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="7b276-135">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="7b276-135">America/Caracas</span></span>

<span data-ttu-id="7b276-136">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="7b276-136">America/Asuncion</span></span>

<span data-ttu-id="7b276-137">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="7b276-137">America/Halifax</span></span>

<span data-ttu-id="7b276-138">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="7b276-138">America/Cuiaba</span></span>

<span data-ttu-id="7b276-139">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="7b276-139">America/La_Paz</span></span>

<span data-ttu-id="7b276-140">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="7b276-140">America/Santiago</span></span>

<span data-ttu-id="7b276-141">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="7b276-141">America/St_Johns</span></span>

<span data-ttu-id="7b276-142">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="7b276-142">America/Sao_Paulo</span></span>

<span data-ttu-id="7b276-143">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="7b276-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="7b276-144">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="7b276-144">America/Cayenne</span></span>

<span data-ttu-id="7b276-145">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="7b276-145">America/Godthab</span></span>

<span data-ttu-id="7b276-146">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="7b276-146">America/Montevideo</span></span>

<span data-ttu-id="7b276-147">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="7b276-147">America/Bahia</span></span>

<span data-ttu-id="7b276-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="7b276-148">Etc/GMT+2</span></span>

<span data-ttu-id="7b276-149">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="7b276-149">Atlantic/Azores</span></span>

<span data-ttu-id="7b276-150">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="7b276-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="7b276-151">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="7b276-151">Africa/Casablanca</span></span>

<span data-ttu-id="7b276-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="7b276-152">Etc/GMT</span></span>

<span data-ttu-id="7b276-153">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="7b276-153">Europe/London</span></span>

<span data-ttu-id="7b276-154">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="7b276-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="7b276-155">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="7b276-155">Europe/Berlin</span></span>

<span data-ttu-id="7b276-156">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="7b276-156">Europe/Budapest</span></span>

<span data-ttu-id="7b276-157">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="7b276-157">Europe/Paris</span></span>

<span data-ttu-id="7b276-158">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="7b276-158">Europe/Warsaw</span></span>

<span data-ttu-id="7b276-159">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="7b276-159">Africa/Lagos</span></span>

<span data-ttu-id="7b276-160">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="7b276-160">Africa/Windhoek</span></span>

<span data-ttu-id="7b276-161">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="7b276-161">Europe/Bucharest</span></span>

<span data-ttu-id="7b276-162">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="7b276-162">Asia/Beirut</span></span>

<span data-ttu-id="7b276-163">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="7b276-163">Africa/Cairo</span></span>

<span data-ttu-id="7b276-164">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="7b276-164">Asia/Damascus</span></span>

<span data-ttu-id="7b276-165">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="7b276-165">Africa/Johannesburg</span></span>

<span data-ttu-id="7b276-166">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="7b276-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="7b276-167">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="7b276-167">Europe/Istanbul</span></span>

<span data-ttu-id="7b276-168">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="7b276-168">Asia/Jerusalem</span></span>

<span data-ttu-id="7b276-169">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="7b276-169">Asia/Amman</span></span>

<span data-ttu-id="7b276-170">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="7b276-170">Asia/Baghdad</span></span>

<span data-ttu-id="7b276-171">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="7b276-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="7b276-172">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="7b276-172">Asia/Riyadh</span></span>

<span data-ttu-id="7b276-173">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="7b276-173">Africa/Nairobi</span></span>

<span data-ttu-id="7b276-174">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="7b276-174">Asia/Tehran</span></span>

<span data-ttu-id="7b276-175">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="7b276-175">Asia/Dubai</span></span>

<span data-ttu-id="7b276-176">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="7b276-176">Asia/Baku</span></span>

<span data-ttu-id="7b276-177">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="7b276-177">Europe/Moscow</span></span>

<span data-ttu-id="7b276-178">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="7b276-178">Indian/Mauritius</span></span>

<span data-ttu-id="7b276-179">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="7b276-179">Asia/Tbilisi</span></span>

<span data-ttu-id="7b276-180">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="7b276-180">Asia/Yerevan</span></span>

<span data-ttu-id="7b276-181">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="7b276-181">Asia/Kabul</span></span>

<span data-ttu-id="7b276-182">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="7b276-182">Asia/Karachi</span></span>

<span data-ttu-id="7b276-183">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="7b276-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="7b276-184">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="7b276-184">Asia/Kolkata</span></span>

<span data-ttu-id="7b276-185">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="7b276-185">Asia/Colombo</span></span>

<span data-ttu-id="7b276-186">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="7b276-186">Asia/Kathmandu</span></span>

<span data-ttu-id="7b276-187">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="7b276-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="7b276-188">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="7b276-188">Asia/Dhaka</span></span>

<span data-ttu-id="7b276-189">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="7b276-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="7b276-190">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="7b276-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="7b276-191">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="7b276-191">Asia/Bangkok</span></span>

<span data-ttu-id="7b276-192">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="7b276-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="7b276-193">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="7b276-193">Asia/Shanghai</span></span>

<span data-ttu-id="7b276-194">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="7b276-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="7b276-195">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="7b276-195">Asia/Singapore</span></span>

<span data-ttu-id="7b276-196">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="7b276-196">Australia/Perth</span></span>

<span data-ttu-id="7b276-197">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="7b276-197">Asia/Taipei</span></span>

<span data-ttu-id="7b276-198">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="7b276-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="7b276-199">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="7b276-199">Asia/Irkutsk</span></span>

<span data-ttu-id="7b276-200">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="7b276-200">Asia/Tokyo</span></span>

<span data-ttu-id="7b276-201">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="7b276-201">Asia/Seoul</span></span>

<span data-ttu-id="7b276-202">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="7b276-202">Australia/Adelaide</span></span>

<span data-ttu-id="7b276-203">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="7b276-203">Australia/Darwin</span></span>

<span data-ttu-id="7b276-204">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="7b276-204">Australia/Brisbane</span></span>

<span data-ttu-id="7b276-205">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="7b276-205">Australia/Sydney</span></span>

<span data-ttu-id="7b276-206">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="7b276-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="7b276-207">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="7b276-207">Australia/Hobart</span></span>

<span data-ttu-id="7b276-208">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="7b276-208">Asia/Yakutsk</span></span>

<span data-ttu-id="7b276-209">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="7b276-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="7b276-210">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="7b276-210">Asia/Vladivostok</span></span>

<span data-ttu-id="7b276-211">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="7b276-211">Pacific/Auckland</span></span>

<span data-ttu-id="7b276-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="7b276-212">Etc/GMT-12</span></span>

<span data-ttu-id="7b276-213">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="7b276-213">Pacific/Fiji</span></span>

<span data-ttu-id="7b276-214">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="7b276-214">Asia/Magadan</span></span>

<span data-ttu-id="7b276-215">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="7b276-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="7b276-216">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="7b276-216">Pacific/Apia</span></span>

<span data-ttu-id="7b276-217">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="7b276-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b276-218">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b276-218">JSON representation</span></span>

<span data-ttu-id="7b276-219">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7b276-219">Here is a JSON representation of the resource</span></span>

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
