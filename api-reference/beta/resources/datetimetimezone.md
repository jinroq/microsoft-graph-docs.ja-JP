---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 28f9956c065e59a0db1ffbd0b82175546d3e5139
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973121"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="92145-103">dateTimeTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92145-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92145-104">特定時点の日付、時刻、およびタイム ゾーンを記述します。</span><span class="sxs-lookup"><span data-stu-id="92145-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="92145-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92145-105">Properties</span></span>
| <span data-ttu-id="92145-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92145-106">Property</span></span>     | <span data-ttu-id="92145-107">型</span><span class="sxs-lookup"><span data-stu-id="92145-107">Type</span></span>   |<span data-ttu-id="92145-108">説明</span><span class="sxs-lookup"><span data-stu-id="92145-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92145-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="92145-109">dateTime</span></span>|<span data-ttu-id="92145-110">String</span><span class="sxs-lookup"><span data-stu-id="92145-110">String</span></span>|<span data-ttu-id="92145-111">特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`)。</span><span class="sxs-lookup"><span data-stu-id="92145-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="92145-112">たとえば、"2019-04-16T09:00:00" とします。</span><span class="sxs-lookup"><span data-stu-id="92145-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="92145-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="92145-113">timeZone</span></span>|<span data-ttu-id="92145-114">String</span><span class="sxs-lookup"><span data-stu-id="92145-114">String</span></span>|<span data-ttu-id="92145-115">タイムゾーン ("太平洋標準時" など) を表します。</span><span class="sxs-lookup"><span data-stu-id="92145-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="92145-116">指定可能な値については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92145-116">See below for possible values.</span></span>|

<span data-ttu-id="92145-117">通常、 **timeZone**プロパティは、 [Windows で現在サポートさ](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones)れている任意のタイムゾーン、および[予定表 API でサポートさ](#additional-time-zones)れている追加のタイムゾーンに設定_でき_ます。</span><span class="sxs-lookup"><span data-stu-id="92145-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="92145-118">**DateTimeTimeZone**をメソッド (イベントの[作成](../api/user-post-events.md)や[更新](../api/event-update.md)など) と組み合わせて使用する場合は、サポートされている実際のタイムゾーンをメモする必要があります。これは小さなサブセットになることがあります。</span><span class="sxs-lookup"><span data-stu-id="92145-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="92145-119">追加のタイムゾーン</span><span class="sxs-lookup"><span data-stu-id="92145-119">Additional time zones</span></span>

<span data-ttu-id="92145-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="92145-120">Etc/GMT+12</span></span>

<span data-ttu-id="92145-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="92145-121">Etc/GMT+11</span></span>

<span data-ttu-id="92145-122">太平洋/ホノルル</span><span class="sxs-lookup"><span data-stu-id="92145-122">Pacific/Honolulu</span></span>

<span data-ttu-id="92145-123">アメリカ/アンカレッジ</span><span class="sxs-lookup"><span data-stu-id="92145-123">America/Anchorage</span></span>

<span data-ttu-id="92145-124">アメリカ/サンタイサベル</span><span class="sxs-lookup"><span data-stu-id="92145-124">America/Santa_Isabel</span></span>

<span data-ttu-id="92145-125">アメリカ/ロサンゼルス</span><span class="sxs-lookup"><span data-stu-id="92145-125">America/Los_Angeles</span></span>

<span data-ttu-id="92145-126">アメリカ/フェニックス</span><span class="sxs-lookup"><span data-stu-id="92145-126">America/Phoenix</span></span>

<span data-ttu-id="92145-127">アメリカ/チワワ</span><span class="sxs-lookup"><span data-stu-id="92145-127">America/Chihuahua</span></span>

<span data-ttu-id="92145-128">アメリカ/デンバー</span><span class="sxs-lookup"><span data-stu-id="92145-128">America/Denver</span></span>

<span data-ttu-id="92145-129">アメリカ/グアテマラ</span><span class="sxs-lookup"><span data-stu-id="92145-129">America/Guatemala</span></span>

<span data-ttu-id="92145-130">アメリカ/シカゴ</span><span class="sxs-lookup"><span data-stu-id="92145-130">America/Chicago</span></span>

<span data-ttu-id="92145-131">アメリカ/メキシコシティ</span><span class="sxs-lookup"><span data-stu-id="92145-131">America/Mexico_City</span></span>

<span data-ttu-id="92145-132">アメリカ/リジャイナ</span><span class="sxs-lookup"><span data-stu-id="92145-132">America/Regina</span></span>

<span data-ttu-id="92145-133">アメリカ/ボゴタ</span><span class="sxs-lookup"><span data-stu-id="92145-133">America/Bogota</span></span>

<span data-ttu-id="92145-134">アメリカ/ニューヨーク</span><span class="sxs-lookup"><span data-stu-id="92145-134">America/New_York</span></span>

<span data-ttu-id="92145-135">アメリカ/インディアナ/インディアナポリス</span><span class="sxs-lookup"><span data-stu-id="92145-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="92145-136">アメリカ/カラカス</span><span class="sxs-lookup"><span data-stu-id="92145-136">America/Caracas</span></span>

<span data-ttu-id="92145-137">アメリカ/アスンシオン</span><span class="sxs-lookup"><span data-stu-id="92145-137">America/Asuncion</span></span>

<span data-ttu-id="92145-138">アメリカ/ハリファックス</span><span class="sxs-lookup"><span data-stu-id="92145-138">America/Halifax</span></span>

<span data-ttu-id="92145-139">アメリカ/クイアバ</span><span class="sxs-lookup"><span data-stu-id="92145-139">America/Cuiaba</span></span>

<span data-ttu-id="92145-140">アメリカ/ラパス</span><span class="sxs-lookup"><span data-stu-id="92145-140">America/La_Paz</span></span>

<span data-ttu-id="92145-141">アメリカ/サンティアゴ</span><span class="sxs-lookup"><span data-stu-id="92145-141">America/Santiago</span></span>

<span data-ttu-id="92145-142">アメリカ/セントジョンズ</span><span class="sxs-lookup"><span data-stu-id="92145-142">America/St_Johns</span></span>

<span data-ttu-id="92145-143">アメリカ/サンパウロ</span><span class="sxs-lookup"><span data-stu-id="92145-143">America/Sao_Paulo</span></span>

<span data-ttu-id="92145-144">アメリカ/アルゼンチン/ブエノスアイレス</span><span class="sxs-lookup"><span data-stu-id="92145-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="92145-145">アメリカ/カイエンヌ</span><span class="sxs-lookup"><span data-stu-id="92145-145">America/Cayenne</span></span>

<span data-ttu-id="92145-146">アメリカ/ゴットホープ</span><span class="sxs-lookup"><span data-stu-id="92145-146">America/Godthab</span></span>

<span data-ttu-id="92145-147">アメリカ/モンテビデオ</span><span class="sxs-lookup"><span data-stu-id="92145-147">America/Montevideo</span></span>

<span data-ttu-id="92145-148">アメリカ/バイア</span><span class="sxs-lookup"><span data-stu-id="92145-148">America/Bahia</span></span>

<span data-ttu-id="92145-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="92145-149">Etc/GMT+2</span></span>

<span data-ttu-id="92145-150">大西洋/アゾレス諸島</span><span class="sxs-lookup"><span data-stu-id="92145-150">Atlantic/Azores</span></span>

<span data-ttu-id="92145-151">大西洋/カーボベルデ</span><span class="sxs-lookup"><span data-stu-id="92145-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="92145-152">アフリカ/カサブランカ</span><span class="sxs-lookup"><span data-stu-id="92145-152">Africa/Casablanca</span></span>

<span data-ttu-id="92145-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="92145-153">Etc/GMT</span></span>

<span data-ttu-id="92145-154">ヨーロッパ/ロンドン</span><span class="sxs-lookup"><span data-stu-id="92145-154">Europe/London</span></span>

<span data-ttu-id="92145-155">大西洋/レイキャビク</span><span class="sxs-lookup"><span data-stu-id="92145-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="92145-156">ヨーロッパ/ベルリン</span><span class="sxs-lookup"><span data-stu-id="92145-156">Europe/Berlin</span></span>

<span data-ttu-id="92145-157">ヨーロッパ/ブダペスト</span><span class="sxs-lookup"><span data-stu-id="92145-157">Europe/Budapest</span></span>

<span data-ttu-id="92145-158">ヨーロッパ/パリ</span><span class="sxs-lookup"><span data-stu-id="92145-158">Europe/Paris</span></span>

<span data-ttu-id="92145-159">ヨーロッパ/ワルシャワ</span><span class="sxs-lookup"><span data-stu-id="92145-159">Europe/Warsaw</span></span>

<span data-ttu-id="92145-160">アフリカ/ラゴス</span><span class="sxs-lookup"><span data-stu-id="92145-160">Africa/Lagos</span></span>

<span data-ttu-id="92145-161">アフリカ/ウィントフック</span><span class="sxs-lookup"><span data-stu-id="92145-161">Africa/Windhoek</span></span>

<span data-ttu-id="92145-162">ヨーロッパ/ブカレスト</span><span class="sxs-lookup"><span data-stu-id="92145-162">Europe/Bucharest</span></span>

<span data-ttu-id="92145-163">アジア/ベイルート</span><span class="sxs-lookup"><span data-stu-id="92145-163">Asia/Beirut</span></span>

<span data-ttu-id="92145-164">アフリカ/カイロ</span><span class="sxs-lookup"><span data-stu-id="92145-164">Africa/Cairo</span></span>

<span data-ttu-id="92145-165">アジア/ダマスカス</span><span class="sxs-lookup"><span data-stu-id="92145-165">Asia/Damascus</span></span>

<span data-ttu-id="92145-166">アフリカ/ヨハネスブルグ</span><span class="sxs-lookup"><span data-stu-id="92145-166">Africa/Johannesburg</span></span>

<span data-ttu-id="92145-167">ヨーロッパ/キエフ</span><span class="sxs-lookup"><span data-stu-id="92145-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="92145-168">ヨーロッパ/イスタンブール</span><span class="sxs-lookup"><span data-stu-id="92145-168">Europe/Istanbul</span></span>

<span data-ttu-id="92145-169">アジア/エルサレム</span><span class="sxs-lookup"><span data-stu-id="92145-169">Asia/Jerusalem</span></span>

<span data-ttu-id="92145-170">アジア/アンマン</span><span class="sxs-lookup"><span data-stu-id="92145-170">Asia/Amman</span></span>

<span data-ttu-id="92145-171">アジア/バグダッド</span><span class="sxs-lookup"><span data-stu-id="92145-171">Asia/Baghdad</span></span>

<span data-ttu-id="92145-172">ヨーロッパ/カリーニングラード</span><span class="sxs-lookup"><span data-stu-id="92145-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="92145-173">アジア/リャド</span><span class="sxs-lookup"><span data-stu-id="92145-173">Asia/Riyadh</span></span>

<span data-ttu-id="92145-174">アフリカ/ナイロビ</span><span class="sxs-lookup"><span data-stu-id="92145-174">Africa/Nairobi</span></span>

<span data-ttu-id="92145-175">アジア/テヘラン</span><span class="sxs-lookup"><span data-stu-id="92145-175">Asia/Tehran</span></span>

<span data-ttu-id="92145-176">アジア/ドバイ</span><span class="sxs-lookup"><span data-stu-id="92145-176">Asia/Dubai</span></span>

<span data-ttu-id="92145-177">アジア/バクー</span><span class="sxs-lookup"><span data-stu-id="92145-177">Asia/Baku</span></span>

<span data-ttu-id="92145-178">ヨーロッパ/モスクワ</span><span class="sxs-lookup"><span data-stu-id="92145-178">Europe/Moscow</span></span>

<span data-ttu-id="92145-179">インド/モーリシャス</span><span class="sxs-lookup"><span data-stu-id="92145-179">Indian/Mauritius</span></span>

<span data-ttu-id="92145-180">アジア/トビリシ</span><span class="sxs-lookup"><span data-stu-id="92145-180">Asia/Tbilisi</span></span>

<span data-ttu-id="92145-181">アジア/エレバン</span><span class="sxs-lookup"><span data-stu-id="92145-181">Asia/Yerevan</span></span>

<span data-ttu-id="92145-182">アジア/カブール</span><span class="sxs-lookup"><span data-stu-id="92145-182">Asia/Kabul</span></span>

<span data-ttu-id="92145-183">アジア/カラチ</span><span class="sxs-lookup"><span data-stu-id="92145-183">Asia/Karachi</span></span>

<span data-ttu-id="92145-184">アジア/タシケント</span><span class="sxs-lookup"><span data-stu-id="92145-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="92145-185">アジア/コルカタ</span><span class="sxs-lookup"><span data-stu-id="92145-185">Asia/Kolkata</span></span>

<span data-ttu-id="92145-186">アジア/コロンボ</span><span class="sxs-lookup"><span data-stu-id="92145-186">Asia/Colombo</span></span>

<span data-ttu-id="92145-187">アジア/カトマンズ</span><span class="sxs-lookup"><span data-stu-id="92145-187">Asia/Kathmandu</span></span>

<span data-ttu-id="92145-188">アジア/アスタナ (アルマトイ)</span><span class="sxs-lookup"><span data-stu-id="92145-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="92145-189">アジア/ダッカ</span><span class="sxs-lookup"><span data-stu-id="92145-189">Asia/Dhaka</span></span>

<span data-ttu-id="92145-190">アジア/エカテリンブルク</span><span class="sxs-lookup"><span data-stu-id="92145-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="92145-191">アジア/ヤンゴン (ラングーン)</span><span class="sxs-lookup"><span data-stu-id="92145-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="92145-192">アジア/バンコク</span><span class="sxs-lookup"><span data-stu-id="92145-192">Asia/Bangkok</span></span>

<span data-ttu-id="92145-193">アジア/ノボシビルスク</span><span class="sxs-lookup"><span data-stu-id="92145-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="92145-194">アジア/上海</span><span class="sxs-lookup"><span data-stu-id="92145-194">Asia/Shanghai</span></span>

<span data-ttu-id="92145-195">アジア/クラスノヤルスク</span><span class="sxs-lookup"><span data-stu-id="92145-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="92145-196">アジア/シンガポール</span><span class="sxs-lookup"><span data-stu-id="92145-196">Asia/Singapore</span></span>

<span data-ttu-id="92145-197">オーストラリア/パース</span><span class="sxs-lookup"><span data-stu-id="92145-197">Australia/Perth</span></span>

<span data-ttu-id="92145-198">アジア/台北</span><span class="sxs-lookup"><span data-stu-id="92145-198">Asia/Taipei</span></span>

<span data-ttu-id="92145-199">アジア/ウランバートル</span><span class="sxs-lookup"><span data-stu-id="92145-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="92145-200">アジア/イルクーツク</span><span class="sxs-lookup"><span data-stu-id="92145-200">Asia/Irkutsk</span></span>

<span data-ttu-id="92145-201">アジア/東京</span><span class="sxs-lookup"><span data-stu-id="92145-201">Asia/Tokyo</span></span>

<span data-ttu-id="92145-202">アジア/ソウル</span><span class="sxs-lookup"><span data-stu-id="92145-202">Asia/Seoul</span></span>

<span data-ttu-id="92145-203">オーストラリア/アデレード</span><span class="sxs-lookup"><span data-stu-id="92145-203">Australia/Adelaide</span></span>

<span data-ttu-id="92145-204">オーストラリア/ダーウィン</span><span class="sxs-lookup"><span data-stu-id="92145-204">Australia/Darwin</span></span>

<span data-ttu-id="92145-205">オーストラリア/ブリスベン</span><span class="sxs-lookup"><span data-stu-id="92145-205">Australia/Brisbane</span></span>

<span data-ttu-id="92145-206">オーストラリア/シドニー</span><span class="sxs-lookup"><span data-stu-id="92145-206">Australia/Sydney</span></span>

<span data-ttu-id="92145-207">太平洋/ポートモレスビー</span><span class="sxs-lookup"><span data-stu-id="92145-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="92145-208">オーストラリア/ホバート</span><span class="sxs-lookup"><span data-stu-id="92145-208">Australia/Hobart</span></span>

<span data-ttu-id="92145-209">アジア/ヤクーツク</span><span class="sxs-lookup"><span data-stu-id="92145-209">Asia/Yakutsk</span></span>

<span data-ttu-id="92145-210">太平洋/ガダルカナル島</span><span class="sxs-lookup"><span data-stu-id="92145-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="92145-211">アジア/ウラジオストク</span><span class="sxs-lookup"><span data-stu-id="92145-211">Asia/Vladivostok</span></span>

<span data-ttu-id="92145-212">太平洋/オークランド</span><span class="sxs-lookup"><span data-stu-id="92145-212">Pacific/Auckland</span></span>

<span data-ttu-id="92145-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="92145-213">Etc/GMT-12</span></span>

<span data-ttu-id="92145-214">太平洋/フィジー</span><span class="sxs-lookup"><span data-stu-id="92145-214">Pacific/Fiji</span></span>

<span data-ttu-id="92145-215">アジア/マガダン</span><span class="sxs-lookup"><span data-stu-id="92145-215">Asia/Magadan</span></span>

<span data-ttu-id="92145-216">太平洋/トンガタプ</span><span class="sxs-lookup"><span data-stu-id="92145-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="92145-217">太平洋/アピア</span><span class="sxs-lookup"><span data-stu-id="92145-217">Pacific/Apia</span></span>

<span data-ttu-id="92145-218">太平洋/クリスマス島</span><span class="sxs-lookup"><span data-stu-id="92145-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="92145-219">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92145-219">JSON representation</span></span>

<span data-ttu-id="92145-220">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="92145-220">Here is a JSON representation of the resource</span></span>

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
