---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Normal
ms.openlocfilehash: 5090edce8d86ff12470cc1bb39f92ef13b42ba15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876070"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="066b9-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="066b9-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="066b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="066b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="066b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="066b9-106">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="066b9-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="066b9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="066b9-107">Properties</span></span>
| <span data-ttu-id="066b9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="066b9-108">Property</span></span>     | <span data-ttu-id="066b9-109">種類</span><span class="sxs-lookup"><span data-stu-id="066b9-109">Type</span></span>   |<span data-ttu-id="066b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="066b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="066b9-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="066b9-111">DateTime</span></span>|<span data-ttu-id="066b9-112">String</span><span class="sxs-lookup"><span data-stu-id="066b9-112">String</span></span>|<span data-ttu-id="066b9-113">特定時点の日付と時刻を組み合わせた表現 (`<date>T<time>`)。</span><span class="sxs-lookup"><span data-stu-id="066b9-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="066b9-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="066b9-114">TimeZone</span></span>|<span data-ttu-id="066b9-115">String</span><span class="sxs-lookup"><span data-stu-id="066b9-115">String</span></span>|<span data-ttu-id="066b9-116">次のいずれかのタイム ゾーン名。</span><span class="sxs-lookup"><span data-stu-id="066b9-116">One of the following time zone names.</span></span>|

<span data-ttu-id="066b9-117">_TimeZone_ プロパティは、Windows でサポートされている任意のタイム ゾーン、および次のタイム ゾーン名に設定できます。</span><span class="sxs-lookup"><span data-stu-id="066b9-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="066b9-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="066b9-118">Etc/GMT+12</span></span>

<span data-ttu-id="066b9-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="066b9-119">Etc/GMT+11</span></span>

<span data-ttu-id="066b9-120">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="066b9-120">Pacific/Honolulu</span></span>

<span data-ttu-id="066b9-121">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="066b9-121">America/Anchorage</span></span>

<span data-ttu-id="066b9-122">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="066b9-122">America/Santa_Isabel</span></span>

<span data-ttu-id="066b9-123">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="066b9-123">America/Los_Angeles</span></span>

<span data-ttu-id="066b9-124">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="066b9-124">America/Phoenix</span></span>

<span data-ttu-id="066b9-125">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="066b9-125">America/Chihuahua</span></span>

<span data-ttu-id="066b9-126">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="066b9-126">America/Denver</span></span>

<span data-ttu-id="066b9-127">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="066b9-127">America/Guatemala</span></span>

<span data-ttu-id="066b9-128">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="066b9-128">America/Chicago</span></span>

<span data-ttu-id="066b9-129">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="066b9-129">America/Mexico_City</span></span>

<span data-ttu-id="066b9-130">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="066b9-130">America/Regina</span></span>

<span data-ttu-id="066b9-131">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="066b9-131">America/Bogota</span></span>

<span data-ttu-id="066b9-132">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="066b9-132">America/New_York</span></span>

<span data-ttu-id="066b9-133">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="066b9-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="066b9-134">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="066b9-134">America/Caracas</span></span>

<span data-ttu-id="066b9-135">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="066b9-135">America/Asuncion</span></span>

<span data-ttu-id="066b9-136">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="066b9-136">America/Halifax</span></span>

<span data-ttu-id="066b9-137">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="066b9-137">America/Cuiaba</span></span>

<span data-ttu-id="066b9-138">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="066b9-138">America/La_Paz</span></span>

<span data-ttu-id="066b9-139">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="066b9-139">America/Santiago</span></span>

<span data-ttu-id="066b9-140">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="066b9-140">America/St_Johns</span></span>

<span data-ttu-id="066b9-141">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="066b9-141">America/Sao_Paulo</span></span>

<span data-ttu-id="066b9-142">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="066b9-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="066b9-143">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="066b9-143">America/Cayenne</span></span>

<span data-ttu-id="066b9-144">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="066b9-144">America/Godthab</span></span>

<span data-ttu-id="066b9-145">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="066b9-145">America/Montevideo</span></span>

<span data-ttu-id="066b9-146">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="066b9-146">America/Bahia</span></span>

<span data-ttu-id="066b9-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="066b9-147">Etc/GMT+2</span></span>

<span data-ttu-id="066b9-148">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="066b9-148">Atlantic/Azores</span></span>

<span data-ttu-id="066b9-149">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="066b9-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="066b9-150">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="066b9-150">Africa/Casablanca</span></span>

<span data-ttu-id="066b9-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="066b9-151">Etc/GMT</span></span>

<span data-ttu-id="066b9-152">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="066b9-152">Europe/London</span></span>

<span data-ttu-id="066b9-153">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="066b9-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="066b9-154">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="066b9-154">Europe/Berlin</span></span>

<span data-ttu-id="066b9-155">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="066b9-155">Europe/Budapest</span></span>

<span data-ttu-id="066b9-156">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="066b9-156">Europe/Paris</span></span>

<span data-ttu-id="066b9-157">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="066b9-157">Europe/Warsaw</span></span>

<span data-ttu-id="066b9-158">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="066b9-158">Africa/Lagos</span></span>

<span data-ttu-id="066b9-159">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="066b9-159">Africa/Windhoek</span></span>

<span data-ttu-id="066b9-160">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="066b9-160">Europe/Bucharest</span></span>

<span data-ttu-id="066b9-161">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="066b9-161">Asia/Beirut</span></span>

<span data-ttu-id="066b9-162">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="066b9-162">Africa/Cairo</span></span>

<span data-ttu-id="066b9-163">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="066b9-163">Asia/Damascus</span></span>

<span data-ttu-id="066b9-164">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="066b9-164">Africa/Johannesburg</span></span>

<span data-ttu-id="066b9-165">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="066b9-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="066b9-166">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="066b9-166">Europe/Istanbul</span></span>

<span data-ttu-id="066b9-167">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="066b9-167">Asia/Jerusalem</span></span>

<span data-ttu-id="066b9-168">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="066b9-168">Asia/Amman</span></span>

<span data-ttu-id="066b9-169">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="066b9-169">Asia/Baghdad</span></span>

<span data-ttu-id="066b9-170">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="066b9-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="066b9-171">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="066b9-171">Asia/Riyadh</span></span>

<span data-ttu-id="066b9-172">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="066b9-172">Africa/Nairobi</span></span>

<span data-ttu-id="066b9-173">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="066b9-173">Asia/Tehran</span></span>

<span data-ttu-id="066b9-174">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="066b9-174">Asia/Dubai</span></span>

<span data-ttu-id="066b9-175">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="066b9-175">Asia/Baku</span></span>

<span data-ttu-id="066b9-176">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="066b9-176">Europe/Moscow</span></span>

<span data-ttu-id="066b9-177">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="066b9-177">Indian/Mauritius</span></span>

<span data-ttu-id="066b9-178">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="066b9-178">Asia/Tbilisi</span></span>

<span data-ttu-id="066b9-179">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="066b9-179">Asia/Yerevan</span></span>

<span data-ttu-id="066b9-180">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="066b9-180">Asia/Kabul</span></span>

<span data-ttu-id="066b9-181">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="066b9-181">Asia/Karachi</span></span>

<span data-ttu-id="066b9-182">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="066b9-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="066b9-183">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="066b9-183">Asia/Kolkata</span></span>

<span data-ttu-id="066b9-184">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="066b9-184">Asia/Colombo</span></span>

<span data-ttu-id="066b9-185">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="066b9-185">Asia/Kathmandu</span></span>

<span data-ttu-id="066b9-186">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="066b9-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="066b9-187">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="066b9-187">Asia/Dhaka</span></span>

<span data-ttu-id="066b9-188">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="066b9-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="066b9-189">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="066b9-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="066b9-190">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="066b9-190">Asia/Bangkok</span></span>

<span data-ttu-id="066b9-191">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="066b9-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="066b9-192">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="066b9-192">Asia/Shanghai</span></span>

<span data-ttu-id="066b9-193">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="066b9-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="066b9-194">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="066b9-194">Asia/Singapore</span></span>

<span data-ttu-id="066b9-195">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="066b9-195">Australia/Perth</span></span>

<span data-ttu-id="066b9-196">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="066b9-196">Asia/Taipei</span></span>

<span data-ttu-id="066b9-197">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="066b9-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="066b9-198">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="066b9-198">Asia/Irkutsk</span></span>

<span data-ttu-id="066b9-199">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="066b9-199">Asia/Tokyo</span></span>

<span data-ttu-id="066b9-200">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="066b9-200">Asia/Seoul</span></span>

<span data-ttu-id="066b9-201">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="066b9-201">Australia/Adelaide</span></span>

<span data-ttu-id="066b9-202">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="066b9-202">Australia/Darwin</span></span>

<span data-ttu-id="066b9-203">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="066b9-203">Australia/Brisbane</span></span>

<span data-ttu-id="066b9-204">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="066b9-204">Australia/Sydney</span></span>

<span data-ttu-id="066b9-205">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="066b9-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="066b9-206">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="066b9-206">Australia/Hobart</span></span>

<span data-ttu-id="066b9-207">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="066b9-207">Asia/Yakutsk</span></span>

<span data-ttu-id="066b9-208">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="066b9-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="066b9-209">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="066b9-209">Asia/Vladivostok</span></span>

<span data-ttu-id="066b9-210">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="066b9-210">Pacific/Auckland</span></span>

<span data-ttu-id="066b9-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="066b9-211">Etc/GMT-12</span></span>

<span data-ttu-id="066b9-212">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="066b9-212">Pacific/Fiji</span></span>

<span data-ttu-id="066b9-213">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="066b9-213">Asia/Magadan</span></span>

<span data-ttu-id="066b9-214">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="066b9-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="066b9-215">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="066b9-215">Pacific/Apia</span></span>

<span data-ttu-id="066b9-216">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="066b9-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="066b9-217">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="066b9-217">JSON representation</span></span>

<span data-ttu-id="066b9-218">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="066b9-218">Here is a JSON representation of the resource</span></span>

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
