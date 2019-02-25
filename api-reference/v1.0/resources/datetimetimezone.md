---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212362"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="efb3e-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="efb3e-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="efb3e-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="efb3e-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="efb3e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efb3e-105">Properties</span></span>
| <span data-ttu-id="efb3e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efb3e-106">Property</span></span>     | <span data-ttu-id="efb3e-107">型</span><span class="sxs-lookup"><span data-stu-id="efb3e-107">Type</span></span>   |<span data-ttu-id="efb3e-108">説明</span><span class="sxs-lookup"><span data-stu-id="efb3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efb3e-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="efb3e-109">dateTime</span></span>|<span data-ttu-id="efb3e-110">String</span><span class="sxs-lookup"><span data-stu-id="efb3e-110">String</span></span>|<span data-ttu-id="efb3e-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`、例 `2017-08-29T04:00:00.0000000`)。</span><span class="sxs-lookup"><span data-stu-id="efb3e-111">A single point of time in a combined date and time representation.</span></span>|
|<span data-ttu-id="efb3e-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="efb3e-112">timeZone</span></span>|<span data-ttu-id="efb3e-113">String</span><span class="sxs-lookup"><span data-stu-id="efb3e-113">String</span></span>|<span data-ttu-id="efb3e-114">次のいずれかのタイム ゾーン名。</span><span class="sxs-lookup"><span data-stu-id="efb3e-114">One of the following time zone names.</span></span>|

<span data-ttu-id="efb3e-115">_TimeZone_ プロパティは、Windows でサポートされている任意のタイム ゾーン、および次のタイム ゾーン名に設定できます。</span><span class="sxs-lookup"><span data-stu-id="efb3e-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="efb3e-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="efb3e-116">Etc/GMT+12</span></span>

<span data-ttu-id="efb3e-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="efb3e-117">Etc/GMT+11</span></span>

<span data-ttu-id="efb3e-118">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="efb3e-118">Pacific/Honolulu</span></span>

<span data-ttu-id="efb3e-119">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="efb3e-119">America/Anchorage</span></span>

<span data-ttu-id="efb3e-120">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="efb3e-120">America/Santa_Isabel</span></span>

<span data-ttu-id="efb3e-121">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="efb3e-121">America/Los_Angeles</span></span>

<span data-ttu-id="efb3e-122">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="efb3e-122">America/Phoenix</span></span>

<span data-ttu-id="efb3e-123">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="efb3e-123">America/Chihuahua</span></span>

<span data-ttu-id="efb3e-124">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="efb3e-124">America/Denver</span></span>

<span data-ttu-id="efb3e-125">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="efb3e-125">America/Guatemala</span></span>

<span data-ttu-id="efb3e-126">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="efb3e-126">America/Chicago</span></span>

<span data-ttu-id="efb3e-127">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="efb3e-127">America/Mexico_City</span></span>

<span data-ttu-id="efb3e-128">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="efb3e-128">America/Regina</span></span>

<span data-ttu-id="efb3e-129">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="efb3e-129">America/Bogota</span></span>

<span data-ttu-id="efb3e-130">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="efb3e-130">America/New_York</span></span>

<span data-ttu-id="efb3e-131">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="efb3e-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="efb3e-132">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="efb3e-132">America/Caracas</span></span>

<span data-ttu-id="efb3e-133">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="efb3e-133">America/Asuncion</span></span>

<span data-ttu-id="efb3e-134">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="efb3e-134">America/Halifax</span></span>

<span data-ttu-id="efb3e-135">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="efb3e-135">America/Cuiaba</span></span>

<span data-ttu-id="efb3e-136">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="efb3e-136">America/La_Paz</span></span>

<span data-ttu-id="efb3e-137">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="efb3e-137">America/Santiago</span></span>

<span data-ttu-id="efb3e-138">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="efb3e-138">America/St_Johns</span></span>

<span data-ttu-id="efb3e-139">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="efb3e-139">America/Sao_Paulo</span></span>

<span data-ttu-id="efb3e-140">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="efb3e-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="efb3e-141">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="efb3e-141">America/Cayenne</span></span>

<span data-ttu-id="efb3e-142">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="efb3e-142">America/Godthab</span></span>

<span data-ttu-id="efb3e-143">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="efb3e-143">America/Montevideo</span></span>

<span data-ttu-id="efb3e-144">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="efb3e-144">America/Bahia</span></span>

<span data-ttu-id="efb3e-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="efb3e-145">Etc/GMT+2</span></span>

<span data-ttu-id="efb3e-146">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="efb3e-146">Atlantic/Azores</span></span>

<span data-ttu-id="efb3e-147">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="efb3e-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="efb3e-148">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="efb3e-148">Africa/Casablanca</span></span>

<span data-ttu-id="efb3e-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="efb3e-149">Etc/GMT</span></span>

<span data-ttu-id="efb3e-150">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="efb3e-150">Europe/London</span></span>

<span data-ttu-id="efb3e-151">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="efb3e-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="efb3e-152">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="efb3e-152">Europe/Berlin</span></span>

<span data-ttu-id="efb3e-153">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="efb3e-153">Europe/Budapest</span></span>

<span data-ttu-id="efb3e-154">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="efb3e-154">Europe/Paris</span></span>

<span data-ttu-id="efb3e-155">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="efb3e-155">Europe/Warsaw</span></span>

<span data-ttu-id="efb3e-156">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="efb3e-156">Africa/Lagos</span></span>

<span data-ttu-id="efb3e-157">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="efb3e-157">Africa/Windhoek</span></span>

<span data-ttu-id="efb3e-158">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="efb3e-158">Europe/Bucharest</span></span>

<span data-ttu-id="efb3e-159">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="efb3e-159">Asia/Beirut</span></span>

<span data-ttu-id="efb3e-160">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="efb3e-160">Africa/Cairo</span></span>

<span data-ttu-id="efb3e-161">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="efb3e-161">Asia/Damascus</span></span>

<span data-ttu-id="efb3e-162">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="efb3e-162">Africa/Johannesburg</span></span>

<span data-ttu-id="efb3e-163">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="efb3e-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="efb3e-164">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="efb3e-164">Europe/Istanbul</span></span>

<span data-ttu-id="efb3e-165">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="efb3e-165">Asia/Jerusalem</span></span>

<span data-ttu-id="efb3e-166">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="efb3e-166">Asia/Amman</span></span>

<span data-ttu-id="efb3e-167">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="efb3e-167">Asia/Baghdad</span></span>

<span data-ttu-id="efb3e-168">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="efb3e-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="efb3e-169">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="efb3e-169">Asia/Riyadh</span></span>

<span data-ttu-id="efb3e-170">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="efb3e-170">Africa/Nairobi</span></span>

<span data-ttu-id="efb3e-171">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="efb3e-171">Asia/Tehran</span></span>

<span data-ttu-id="efb3e-172">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="efb3e-172">Asia/Dubai</span></span>

<span data-ttu-id="efb3e-173">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="efb3e-173">Asia/Baku</span></span>

<span data-ttu-id="efb3e-174">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="efb3e-174">Europe/Moscow</span></span>

<span data-ttu-id="efb3e-175">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="efb3e-175">Indian/Mauritius</span></span>

<span data-ttu-id="efb3e-176">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="efb3e-176">Asia/Tbilisi</span></span>

<span data-ttu-id="efb3e-177">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="efb3e-177">Asia/Yerevan</span></span>

<span data-ttu-id="efb3e-178">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="efb3e-178">Asia/Kabul</span></span>

<span data-ttu-id="efb3e-179">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="efb3e-179">Asia/Karachi</span></span>

<span data-ttu-id="efb3e-180">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="efb3e-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="efb3e-181">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="efb3e-181">Asia/Kolkata</span></span>

<span data-ttu-id="efb3e-182">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="efb3e-182">Asia/Colombo</span></span>

<span data-ttu-id="efb3e-183">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="efb3e-183">Asia/Kathmandu</span></span>

<span data-ttu-id="efb3e-184">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="efb3e-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="efb3e-185">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="efb3e-185">Asia/Dhaka</span></span>

<span data-ttu-id="efb3e-186">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="efb3e-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="efb3e-187">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="efb3e-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="efb3e-188">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="efb3e-188">Asia/Bangkok</span></span>

<span data-ttu-id="efb3e-189">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="efb3e-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="efb3e-190">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="efb3e-190">Asia/Shanghai</span></span>

<span data-ttu-id="efb3e-191">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="efb3e-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="efb3e-192">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="efb3e-192">Asia/Singapore</span></span>

<span data-ttu-id="efb3e-193">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="efb3e-193">Australia/Perth</span></span>

<span data-ttu-id="efb3e-194">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="efb3e-194">Asia/Taipei</span></span>

<span data-ttu-id="efb3e-195">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="efb3e-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="efb3e-196">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="efb3e-196">Asia/Irkutsk</span></span>

<span data-ttu-id="efb3e-197">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="efb3e-197">Asia/Tokyo</span></span>

<span data-ttu-id="efb3e-198">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="efb3e-198">Asia/Seoul</span></span>

<span data-ttu-id="efb3e-199">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="efb3e-199">Australia/Adelaide</span></span>

<span data-ttu-id="efb3e-200">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="efb3e-200">Australia/Darwin</span></span>

<span data-ttu-id="efb3e-201">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="efb3e-201">Australia/Brisbane</span></span>

<span data-ttu-id="efb3e-202">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="efb3e-202">Australia/Sydney</span></span>

<span data-ttu-id="efb3e-203">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="efb3e-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="efb3e-204">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="efb3e-204">Australia/Hobart</span></span>

<span data-ttu-id="efb3e-205">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="efb3e-205">Asia/Yakutsk</span></span>

<span data-ttu-id="efb3e-206">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="efb3e-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="efb3e-207">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="efb3e-207">Asia/Vladivostok</span></span>

<span data-ttu-id="efb3e-208">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="efb3e-208">Pacific/Auckland</span></span>

<span data-ttu-id="efb3e-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="efb3e-209">Etc/GMT-12</span></span>

<span data-ttu-id="efb3e-210">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="efb3e-210">Pacific/Fiji</span></span>

<span data-ttu-id="efb3e-211">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="efb3e-211">Asia/Magadan</span></span>

<span data-ttu-id="efb3e-212">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="efb3e-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="efb3e-213">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="efb3e-213">Pacific/Apia</span></span>

<span data-ttu-id="efb3e-214">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="efb3e-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="efb3e-215">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="efb3e-215">JSON representation</span></span>

<span data-ttu-id="efb3e-216">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="efb3e-216">Here is a JSON representation of the resource</span></span>

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
