---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574772"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="cc757-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc757-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="cc757-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="cc757-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="cc757-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc757-105">Properties</span></span>
| <span data-ttu-id="cc757-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc757-106">Property</span></span>     | <span data-ttu-id="cc757-107">型</span><span class="sxs-lookup"><span data-stu-id="cc757-107">Type</span></span>   |<span data-ttu-id="cc757-108">説明</span><span class="sxs-lookup"><span data-stu-id="cc757-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc757-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="cc757-109">dateTime</span></span>|<span data-ttu-id="cc757-110">String</span><span class="sxs-lookup"><span data-stu-id="cc757-110">String</span></span>|<span data-ttu-id="cc757-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`、例 `2017-08-29T04:00:00.0000000`)。</span><span class="sxs-lookup"><span data-stu-id="cc757-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="cc757-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="cc757-112">timeZone</span></span>|<span data-ttu-id="cc757-113">String</span><span class="sxs-lookup"><span data-stu-id="cc757-113">String</span></span>|<span data-ttu-id="cc757-114">次のいずれかのタイム ゾーン名。</span><span class="sxs-lookup"><span data-stu-id="cc757-114">One of the following time zone names.</span></span>|

<span data-ttu-id="cc757-115">_TimeZone_ プロパティは、Windows でサポートされている任意のタイム ゾーン、および次のタイム ゾーン名に設定できます。</span><span class="sxs-lookup"><span data-stu-id="cc757-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="cc757-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="cc757-116">Etc/GMT+12</span></span>

<span data-ttu-id="cc757-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="cc757-117">Etc/GMT+11</span></span>

<span data-ttu-id="cc757-118">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="cc757-118">Pacific/Honolulu</span></span>

<span data-ttu-id="cc757-119">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="cc757-119">America/Anchorage</span></span>

<span data-ttu-id="cc757-120">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="cc757-120">America/Santa_Isabel</span></span>

<span data-ttu-id="cc757-121">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="cc757-121">America/Los_Angeles</span></span>

<span data-ttu-id="cc757-122">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="cc757-122">America/Phoenix</span></span>

<span data-ttu-id="cc757-123">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="cc757-123">America/Chihuahua</span></span>

<span data-ttu-id="cc757-124">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="cc757-124">America/Denver</span></span>

<span data-ttu-id="cc757-125">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="cc757-125">America/Guatemala</span></span>

<span data-ttu-id="cc757-126">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="cc757-126">America/Chicago</span></span>

<span data-ttu-id="cc757-127">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="cc757-127">America/Mexico_City</span></span>

<span data-ttu-id="cc757-128">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="cc757-128">America/Regina</span></span>

<span data-ttu-id="cc757-129">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="cc757-129">America/Bogota</span></span>

<span data-ttu-id="cc757-130">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="cc757-130">America/New_York</span></span>

<span data-ttu-id="cc757-131">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="cc757-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="cc757-132">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="cc757-132">America/Caracas</span></span>

<span data-ttu-id="cc757-133">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="cc757-133">America/Asuncion</span></span>

<span data-ttu-id="cc757-134">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="cc757-134">America/Halifax</span></span>

<span data-ttu-id="cc757-135">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="cc757-135">America/Cuiaba</span></span>

<span data-ttu-id="cc757-136">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="cc757-136">America/La_Paz</span></span>

<span data-ttu-id="cc757-137">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="cc757-137">America/Santiago</span></span>

<span data-ttu-id="cc757-138">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="cc757-138">America/St_Johns</span></span>

<span data-ttu-id="cc757-139">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="cc757-139">America/Sao_Paulo</span></span>

<span data-ttu-id="cc757-140">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="cc757-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="cc757-141">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="cc757-141">America/Cayenne</span></span>

<span data-ttu-id="cc757-142">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="cc757-142">America/Godthab</span></span>

<span data-ttu-id="cc757-143">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="cc757-143">America/Montevideo</span></span>

<span data-ttu-id="cc757-144">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="cc757-144">America/Bahia</span></span>

<span data-ttu-id="cc757-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="cc757-145">Etc/GMT+2</span></span>

<span data-ttu-id="cc757-146">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="cc757-146">Atlantic/Azores</span></span>

<span data-ttu-id="cc757-147">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="cc757-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="cc757-148">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="cc757-148">Africa/Casablanca</span></span>

<span data-ttu-id="cc757-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="cc757-149">Etc/GMT</span></span>

<span data-ttu-id="cc757-150">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="cc757-150">Europe/London</span></span>

<span data-ttu-id="cc757-151">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="cc757-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="cc757-152">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="cc757-152">Europe/Berlin</span></span>

<span data-ttu-id="cc757-153">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="cc757-153">Europe/Budapest</span></span>

<span data-ttu-id="cc757-154">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="cc757-154">Europe/Paris</span></span>

<span data-ttu-id="cc757-155">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="cc757-155">Europe/Warsaw</span></span>

<span data-ttu-id="cc757-156">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="cc757-156">Africa/Lagos</span></span>

<span data-ttu-id="cc757-157">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="cc757-157">Africa/Windhoek</span></span>

<span data-ttu-id="cc757-158">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="cc757-158">Europe/Bucharest</span></span>

<span data-ttu-id="cc757-159">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="cc757-159">Asia/Beirut</span></span>

<span data-ttu-id="cc757-160">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="cc757-160">Africa/Cairo</span></span>

<span data-ttu-id="cc757-161">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="cc757-161">Asia/Damascus</span></span>

<span data-ttu-id="cc757-162">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="cc757-162">Africa/Johannesburg</span></span>

<span data-ttu-id="cc757-163">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="cc757-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="cc757-164">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="cc757-164">Europe/Istanbul</span></span>

<span data-ttu-id="cc757-165">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="cc757-165">Asia/Jerusalem</span></span>

<span data-ttu-id="cc757-166">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="cc757-166">Asia/Amman</span></span>

<span data-ttu-id="cc757-167">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="cc757-167">Asia/Baghdad</span></span>

<span data-ttu-id="cc757-168">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="cc757-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="cc757-169">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="cc757-169">Asia/Riyadh</span></span>

<span data-ttu-id="cc757-170">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="cc757-170">Africa/Nairobi</span></span>

<span data-ttu-id="cc757-171">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="cc757-171">Asia/Tehran</span></span>

<span data-ttu-id="cc757-172">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="cc757-172">Asia/Dubai</span></span>

<span data-ttu-id="cc757-173">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="cc757-173">Asia/Baku</span></span>

<span data-ttu-id="cc757-174">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="cc757-174">Europe/Moscow</span></span>

<span data-ttu-id="cc757-175">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="cc757-175">Indian/Mauritius</span></span>

<span data-ttu-id="cc757-176">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="cc757-176">Asia/Tbilisi</span></span>

<span data-ttu-id="cc757-177">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="cc757-177">Asia/Yerevan</span></span>

<span data-ttu-id="cc757-178">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="cc757-178">Asia/Kabul</span></span>

<span data-ttu-id="cc757-179">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="cc757-179">Asia/Karachi</span></span>

<span data-ttu-id="cc757-180">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="cc757-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="cc757-181">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="cc757-181">Asia/Kolkata</span></span>

<span data-ttu-id="cc757-182">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="cc757-182">Asia/Colombo</span></span>

<span data-ttu-id="cc757-183">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="cc757-183">Asia/Kathmandu</span></span>

<span data-ttu-id="cc757-184">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="cc757-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="cc757-185">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="cc757-185">Asia/Dhaka</span></span>

<span data-ttu-id="cc757-186">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="cc757-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="cc757-187">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="cc757-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="cc757-188">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="cc757-188">Asia/Bangkok</span></span>

<span data-ttu-id="cc757-189">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="cc757-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="cc757-190">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="cc757-190">Asia/Shanghai</span></span>

<span data-ttu-id="cc757-191">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="cc757-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="cc757-192">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="cc757-192">Asia/Singapore</span></span>

<span data-ttu-id="cc757-193">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="cc757-193">Australia/Perth</span></span>

<span data-ttu-id="cc757-194">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="cc757-194">Asia/Taipei</span></span>

<span data-ttu-id="cc757-195">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="cc757-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="cc757-196">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="cc757-196">Asia/Irkutsk</span></span>

<span data-ttu-id="cc757-197">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="cc757-197">Asia/Tokyo</span></span>

<span data-ttu-id="cc757-198">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="cc757-198">Asia/Seoul</span></span>

<span data-ttu-id="cc757-199">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="cc757-199">Australia/Adelaide</span></span>

<span data-ttu-id="cc757-200">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="cc757-200">Australia/Darwin</span></span>

<span data-ttu-id="cc757-201">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="cc757-201">Australia/Brisbane</span></span>

<span data-ttu-id="cc757-202">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="cc757-202">Australia/Sydney</span></span>

<span data-ttu-id="cc757-203">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="cc757-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="cc757-204">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="cc757-204">Australia/Hobart</span></span>

<span data-ttu-id="cc757-205">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="cc757-205">Asia/Yakutsk</span></span>

<span data-ttu-id="cc757-206">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="cc757-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="cc757-207">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="cc757-207">Asia/Vladivostok</span></span>

<span data-ttu-id="cc757-208">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="cc757-208">Pacific/Auckland</span></span>

<span data-ttu-id="cc757-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="cc757-209">Etc/GMT-12</span></span>

<span data-ttu-id="cc757-210">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="cc757-210">Pacific/Fiji</span></span>

<span data-ttu-id="cc757-211">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="cc757-211">Asia/Magadan</span></span>

<span data-ttu-id="cc757-212">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="cc757-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="cc757-213">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="cc757-213">Pacific/Apia</span></span>

<span data-ttu-id="cc757-214">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="cc757-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc757-215">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc757-215">JSON representation</span></span>

<span data-ttu-id="cc757-216">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="cc757-216">Here is a JSON representation of the resource</span></span>

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
