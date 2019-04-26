---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Normal
ms.openlocfilehash: 4bf62081d190e3af031d305c7db7f64d606926b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340964"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="ceebb-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ceebb-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceebb-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="ceebb-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="ceebb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceebb-105">Properties</span></span>
| <span data-ttu-id="ceebb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceebb-106">Property</span></span>     | <span data-ttu-id="ceebb-107">型</span><span class="sxs-lookup"><span data-stu-id="ceebb-107">Type</span></span>   |<span data-ttu-id="ceebb-108">説明</span><span class="sxs-lookup"><span data-stu-id="ceebb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceebb-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="ceebb-109">dateTime</span></span>|<span data-ttu-id="ceebb-110">String</span><span class="sxs-lookup"><span data-stu-id="ceebb-110">String</span></span>|<span data-ttu-id="ceebb-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`)。</span><span class="sxs-lookup"><span data-stu-id="ceebb-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="ceebb-112">たとえば、"2019-04-16t09:00:00" とします。</span><span class="sxs-lookup"><span data-stu-id="ceebb-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="ceebb-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="ceebb-113">timeZone</span></span>|<span data-ttu-id="ceebb-114">String</span><span class="sxs-lookup"><span data-stu-id="ceebb-114">String</span></span>|<span data-ttu-id="ceebb-115">次に示すようなタイムゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="ceebb-115">A time zone name as described below.</span></span>|

<span data-ttu-id="ceebb-116">**timeZone**プロパティは、Windows でサポートされている任意のタイムゾーン、および次のタイムゾーン名に設定できます。</span><span class="sxs-lookup"><span data-stu-id="ceebb-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="ceebb-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="ceebb-117">Etc/GMT+12</span></span>

<span data-ttu-id="ceebb-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="ceebb-118">Etc/GMT+11</span></span>

<span data-ttu-id="ceebb-119">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="ceebb-119">Pacific/Honolulu</span></span>

<span data-ttu-id="ceebb-120">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="ceebb-120">America/Anchorage</span></span>

<span data-ttu-id="ceebb-121">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="ceebb-121">America/Santa_Isabel</span></span>

<span data-ttu-id="ceebb-122">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="ceebb-122">America/Los_Angeles</span></span>

<span data-ttu-id="ceebb-123">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="ceebb-123">America/Phoenix</span></span>

<span data-ttu-id="ceebb-124">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="ceebb-124">America/Chihuahua</span></span>

<span data-ttu-id="ceebb-125">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="ceebb-125">America/Denver</span></span>

<span data-ttu-id="ceebb-126">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="ceebb-126">America/Guatemala</span></span>

<span data-ttu-id="ceebb-127">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="ceebb-127">America/Chicago</span></span>

<span data-ttu-id="ceebb-128">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="ceebb-128">America/Mexico_City</span></span>

<span data-ttu-id="ceebb-129">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="ceebb-129">America/Regina</span></span>

<span data-ttu-id="ceebb-130">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="ceebb-130">America/Bogota</span></span>

<span data-ttu-id="ceebb-131">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="ceebb-131">America/New_York</span></span>

<span data-ttu-id="ceebb-132">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="ceebb-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="ceebb-133">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="ceebb-133">America/Caracas</span></span>

<span data-ttu-id="ceebb-134">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="ceebb-134">America/Asuncion</span></span>

<span data-ttu-id="ceebb-135">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="ceebb-135">America/Halifax</span></span>

<span data-ttu-id="ceebb-136">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="ceebb-136">America/Cuiaba</span></span>

<span data-ttu-id="ceebb-137">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="ceebb-137">America/La_Paz</span></span>

<span data-ttu-id="ceebb-138">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="ceebb-138">America/Santiago</span></span>

<span data-ttu-id="ceebb-139">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="ceebb-139">America/St_Johns</span></span>

<span data-ttu-id="ceebb-140">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="ceebb-140">America/Sao_Paulo</span></span>

<span data-ttu-id="ceebb-141">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="ceebb-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="ceebb-142">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="ceebb-142">America/Cayenne</span></span>

<span data-ttu-id="ceebb-143">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="ceebb-143">America/Godthab</span></span>

<span data-ttu-id="ceebb-144">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="ceebb-144">America/Montevideo</span></span>

<span data-ttu-id="ceebb-145">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="ceebb-145">America/Bahia</span></span>

<span data-ttu-id="ceebb-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="ceebb-146">Etc/GMT+2</span></span>

<span data-ttu-id="ceebb-147">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="ceebb-147">Atlantic/Azores</span></span>

<span data-ttu-id="ceebb-148">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="ceebb-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="ceebb-149">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="ceebb-149">Africa/Casablanca</span></span>

<span data-ttu-id="ceebb-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="ceebb-150">Etc/GMT</span></span>

<span data-ttu-id="ceebb-151">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="ceebb-151">Europe/London</span></span>

<span data-ttu-id="ceebb-152">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="ceebb-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="ceebb-153">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="ceebb-153">Europe/Berlin</span></span>

<span data-ttu-id="ceebb-154">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="ceebb-154">Europe/Budapest</span></span>

<span data-ttu-id="ceebb-155">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="ceebb-155">Europe/Paris</span></span>

<span data-ttu-id="ceebb-156">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="ceebb-156">Europe/Warsaw</span></span>

<span data-ttu-id="ceebb-157">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="ceebb-157">Africa/Lagos</span></span>

<span data-ttu-id="ceebb-158">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="ceebb-158">Africa/Windhoek</span></span>

<span data-ttu-id="ceebb-159">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="ceebb-159">Europe/Bucharest</span></span>

<span data-ttu-id="ceebb-160">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="ceebb-160">Asia/Beirut</span></span>

<span data-ttu-id="ceebb-161">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="ceebb-161">Africa/Cairo</span></span>

<span data-ttu-id="ceebb-162">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="ceebb-162">Asia/Damascus</span></span>

<span data-ttu-id="ceebb-163">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="ceebb-163">Africa/Johannesburg</span></span>

<span data-ttu-id="ceebb-164">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="ceebb-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="ceebb-165">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="ceebb-165">Europe/Istanbul</span></span>

<span data-ttu-id="ceebb-166">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="ceebb-166">Asia/Jerusalem</span></span>

<span data-ttu-id="ceebb-167">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="ceebb-167">Asia/Amman</span></span>

<span data-ttu-id="ceebb-168">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="ceebb-168">Asia/Baghdad</span></span>

<span data-ttu-id="ceebb-169">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="ceebb-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="ceebb-170">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="ceebb-170">Asia/Riyadh</span></span>

<span data-ttu-id="ceebb-171">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="ceebb-171">Africa/Nairobi</span></span>

<span data-ttu-id="ceebb-172">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="ceebb-172">Asia/Tehran</span></span>

<span data-ttu-id="ceebb-173">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="ceebb-173">Asia/Dubai</span></span>

<span data-ttu-id="ceebb-174">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="ceebb-174">Asia/Baku</span></span>

<span data-ttu-id="ceebb-175">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="ceebb-175">Europe/Moscow</span></span>

<span data-ttu-id="ceebb-176">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="ceebb-176">Indian/Mauritius</span></span>

<span data-ttu-id="ceebb-177">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="ceebb-177">Asia/Tbilisi</span></span>

<span data-ttu-id="ceebb-178">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="ceebb-178">Asia/Yerevan</span></span>

<span data-ttu-id="ceebb-179">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="ceebb-179">Asia/Kabul</span></span>

<span data-ttu-id="ceebb-180">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="ceebb-180">Asia/Karachi</span></span>

<span data-ttu-id="ceebb-181">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="ceebb-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="ceebb-182">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="ceebb-182">Asia/Kolkata</span></span>

<span data-ttu-id="ceebb-183">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="ceebb-183">Asia/Colombo</span></span>

<span data-ttu-id="ceebb-184">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="ceebb-184">Asia/Kathmandu</span></span>

<span data-ttu-id="ceebb-185">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="ceebb-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="ceebb-186">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="ceebb-186">Asia/Dhaka</span></span>

<span data-ttu-id="ceebb-187">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="ceebb-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="ceebb-188">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="ceebb-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="ceebb-189">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="ceebb-189">Asia/Bangkok</span></span>

<span data-ttu-id="ceebb-190">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="ceebb-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="ceebb-191">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="ceebb-191">Asia/Shanghai</span></span>

<span data-ttu-id="ceebb-192">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="ceebb-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="ceebb-193">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="ceebb-193">Asia/Singapore</span></span>

<span data-ttu-id="ceebb-194">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="ceebb-194">Australia/Perth</span></span>

<span data-ttu-id="ceebb-195">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="ceebb-195">Asia/Taipei</span></span>

<span data-ttu-id="ceebb-196">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="ceebb-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="ceebb-197">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="ceebb-197">Asia/Irkutsk</span></span>

<span data-ttu-id="ceebb-198">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="ceebb-198">Asia/Tokyo</span></span>

<span data-ttu-id="ceebb-199">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="ceebb-199">Asia/Seoul</span></span>

<span data-ttu-id="ceebb-200">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="ceebb-200">Australia/Adelaide</span></span>

<span data-ttu-id="ceebb-201">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="ceebb-201">Australia/Darwin</span></span>

<span data-ttu-id="ceebb-202">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="ceebb-202">Australia/Brisbane</span></span>

<span data-ttu-id="ceebb-203">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="ceebb-203">Australia/Sydney</span></span>

<span data-ttu-id="ceebb-204">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="ceebb-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="ceebb-205">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="ceebb-205">Australia/Hobart</span></span>

<span data-ttu-id="ceebb-206">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="ceebb-206">Asia/Yakutsk</span></span>

<span data-ttu-id="ceebb-207">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="ceebb-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="ceebb-208">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="ceebb-208">Asia/Vladivostok</span></span>

<span data-ttu-id="ceebb-209">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="ceebb-209">Pacific/Auckland</span></span>

<span data-ttu-id="ceebb-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="ceebb-210">Etc/GMT-12</span></span>

<span data-ttu-id="ceebb-211">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="ceebb-211">Pacific/Fiji</span></span>

<span data-ttu-id="ceebb-212">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="ceebb-212">Asia/Magadan</span></span>

<span data-ttu-id="ceebb-213">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="ceebb-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="ceebb-214">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="ceebb-214">Pacific/Apia</span></span>

<span data-ttu-id="ceebb-215">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="ceebb-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceebb-216">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ceebb-216">JSON representation</span></span>

<span data-ttu-id="ceebb-217">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ceebb-217">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
