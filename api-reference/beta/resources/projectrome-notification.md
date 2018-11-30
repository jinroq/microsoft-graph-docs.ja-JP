---
title: 通知リソースの種類
description: '指定したユーザーを対象とするアプリケーション ・ サーバによって提供される通知を表します。 通知は、Microsoft Graph で格納され、ユーザーによって所有されている端点を別のデバイスに配布されます。 '
ms.openlocfilehash: dfcff69fd51ffa8993c0d570883e04a69371fb85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073216"
---
# <a name="notification-resource-type"></a><span data-ttu-id="bfacc-104">通知リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfacc-104">notification resource type</span></span>
> <span data-ttu-id="bfacc-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bfacc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfacc-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfacc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfacc-107">指定したユーザーを対象とするアプリケーション ・ サーバによって提供される通知を表します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-107">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="bfacc-108">通知は、Microsoft Graph で格納され、ユーザーによって所有されている端点を別のデバイスに配布されます。</span><span class="sxs-lookup"><span data-stu-id="bfacc-108">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="bfacc-109">通知には、Windows、Android、iOS プラットフォームを含む、オペレーティング システムによって解釈可能なメッセージ ボックスによる通知のペイロードを指定できます。</span><span class="sxs-lookup"><span data-stu-id="bfacc-109">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="bfacc-110">通常、視覚的に通知が生成される元のデータ ペイロードのコンテンツに対応する UI の – すべてのデバイスに、app のクライアントは、対応するユーザーを決定し、データ ペイロードに配信し、処理が発生することもできます。ローカルにします。</span><span class="sxs-lookup"><span data-stu-id="bfacc-110">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="bfacc-111">ユーザーは、視覚的に通知の動作と、アプリケーション クライアントことができますし、SDK を使用クライアント側プロジェクト ローマを閉じるよう通知をマークすることによって、graph のフィード対応する通知の状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-111">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="bfacc-112">更新プログラムはアプリケーションのクライアント エンドポイントでは、配布して、クライアントこの変化に対応などの冗長な情報を見ることからユーザーを防ぐために通知を無視すれば。</span><span class="sxs-lookup"><span data-stu-id="bfacc-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="bfacc-113">後で (非表示としてマークされます) の後も期限切れ前に、アプリケーションのクライアントを同じ通知リソースにアクセスできる[プロジェクトのローマの SDK](https://github.com/Microsoft/project-rome)を使用して、通知の履歴とします。</span><span class="sxs-lookup"><span data-stu-id="bfacc-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="bfacc-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="bfacc-114">Methods</span></span>
|<span data-ttu-id="bfacc-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="bfacc-115">Method</span></span> | <span data-ttu-id="bfacc-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bfacc-116">Return Type</span></span> | <span data-ttu-id="bfacc-117">説明</span><span class="sxs-lookup"><span data-stu-id="bfacc-117">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="bfacc-118">通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-118">Create notification</span></span>](../api/projectrome-notification-post.md) | [<span data-ttu-id="bfacc-119">通知</span><span class="sxs-lookup"><span data-stu-id="bfacc-119">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="bfacc-120">作成し、通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-120">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfacc-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfacc-121">Properties</span></span>
|<span data-ttu-id="bfacc-122">名前</span><span class="sxs-lookup"><span data-stu-id="bfacc-122">Name</span></span> | <span data-ttu-id="bfacc-123">型</span><span class="sxs-lookup"><span data-stu-id="bfacc-123">Type</span></span> | <span data-ttu-id="bfacc-124">説明</span><span class="sxs-lookup"><span data-stu-id="bfacc-124">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="bfacc-125">targetHostName</span><span class="sxs-lookup"><span data-stu-id="bfacc-125">targetHostName</span></span> | <span data-ttu-id="bfacc-126">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-126">String</span></span> | <span data-ttu-id="bfacc-127">呼び出し元のサービスが特定のユーザーに対して、通知を投稿するのにはアプリケーションのホスト名を表します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-127">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="bfacc-128">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="bfacc-128">appNotificationId</span></span> | <span data-ttu-id="bfacc-129">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-129">String</span></span> | <span data-ttu-id="bfacc-130">識別し、個々 の通知を対象に使用する通知のアプリケーション サーバで設定する一意の id。</span><span class="sxs-lookup"><span data-stu-id="bfacc-130">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="bfacc-131">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfacc-131">expirationDateTime</span></span> | <span data-ttu-id="bfacc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfacc-132">DateTimeOffset</span></span> | <span data-ttu-id="bfacc-133">有効期限の時刻を設定、ユーザーへの通知の上、時間は、通知 Graph フィード通知ストアから完全に削除され、通知履歴の一部ではありません。</span><span class="sxs-lookup"><span data-stu-id="bfacc-133">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="bfacc-134">最大値は、30 日間です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-134">Max value is 30 days.</span></span> |
| <span data-ttu-id="bfacc-135">payload</span><span class="sxs-lookup"><span data-stu-id="bfacc-135">payload</span></span> | <span data-ttu-id="bfacc-136">Edm.ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bfacc-136">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfacc-137">提供され、この通知を受け取るアプリケーションのクライアントによって消費される raw またはビジュアルのユーザーの通知のデータ コンテンツです。</span><span class="sxs-lookup"><span data-stu-id="bfacc-137">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="bfacc-138">payload.rawContent</span><span class="sxs-lookup"><span data-stu-id="bfacc-138">payload.rawContent</span></span> | <span data-ttu-id="bfacc-139">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-139">String</span></span> | <span data-ttu-id="bfacc-140">提供され、この通知を受け取るアプリケーションのクライアントによって消費されることを示す生のユーザー通知の通知の内容です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-140">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="bfacc-141">投稿の通知要求を有効にする Payload.RawContent と Payload.VisualContent の少なくとも 1 つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfacc-141">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="bfacc-142">payload.visual</span><span class="sxs-lookup"><span data-stu-id="bfacc-142">payload.visual</span></span> | <span data-ttu-id="bfacc-143">Edm.ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bfacc-143">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfacc-144">モバイル プラットフォームごとに通知のプラットフォームで使用され、ユーザーに表示する、ビジュアルなユーザー通知のビジュアルのコンテンツです。</span><span class="sxs-lookup"><span data-stu-id="bfacc-144">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="bfacc-145">投稿の通知要求を有効にするコンテンツと VisualContent の少なくとも 1 つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfacc-145">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="bfacc-146">payload.visual.title</span><span class="sxs-lookup"><span data-stu-id="bfacc-146">payload.visual.title</span></span> | <span data-ttu-id="bfacc-147">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-147">String</span></span> | <span data-ttu-id="bfacc-148">ビジュアルなユーザー通知のタイトル。</span><span class="sxs-lookup"><span data-stu-id="bfacc-148">The title of a visual user notification.</span></span> <span data-ttu-id="bfacc-149">タイトルまたは本文のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-149">Must have either title or body.</span></span> |
| <span data-ttu-id="bfacc-150">payload.visual.body</span><span class="sxs-lookup"><span data-stu-id="bfacc-150">payload.visual.body</span></span> | <span data-ttu-id="bfacc-151">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-151">String</span></span> | <span data-ttu-id="bfacc-152">ビジュアルなユーザー通知の本文です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-152">The body of a visual user notification.</span></span> <span data-ttu-id="bfacc-153">タイトルまたは本文のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-153">Must have either title or body.</span></span> |
| <span data-ttu-id="bfacc-154">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="bfacc-154">displayTimeToLive</span></span> | <span data-ttu-id="bfacc-155">整数型 (Int)</span><span class="sxs-lookup"><span data-stu-id="bfacc-155">Int</span></span> | <span data-ttu-id="bfacc-156">時間 (秒) この通知の内容のままで各プラットフォームの通知のビューアーを設定します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-156">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="bfacc-157">たとえば、通知が配信されると Windows のデバイスに、このプロパティの値に渡されます ToastNotification.ExpirationTime は、どのくらいの時間、トースト通知は常にユーザーの Windows アクション センターで決定します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-157">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="bfacc-158">priority</span><span class="sxs-lookup"><span data-stu-id="bfacc-158">priority</span></span> | <span data-ttu-id="bfacc-159">EnumType</span><span class="sxs-lookup"><span data-stu-id="bfacc-159">EnumType</span></span> | <span data-ttu-id="bfacc-160">生のユーザーの通知の優先順位を示します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-160">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="bfacc-161">既定で優先度の高い視覚的な通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="bfacc-161">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="bfacc-162">有効な値は、最低額です。</span><span class="sxs-lookup"><span data-stu-id="bfacc-162">Valid values are High and Low.</span></span> |
| <span data-ttu-id="bfacc-163">グループ名</span><span class="sxs-lookup"><span data-stu-id="bfacc-163">groupName</span></span> | <span data-ttu-id="bfacc-164">String</span><span class="sxs-lookup"><span data-stu-id="bfacc-164">String</span></span> | <span data-ttu-id="bfacc-165">この通知が所属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="bfacc-165">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="bfacc-166">通知をグループ化するための開発者によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="bfacc-166">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="bfacc-167">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="bfacc-167">targetPolicy</span></span> | <span data-ttu-id="bfacc-168">Edm.ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bfacc-168">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfacc-169">ターゲット ポリシー オブジェクトは、さまざまなレベルの 2 つのエンドポイントの種類 (Windows、iOS および Android) の対象とする、および対象とする、(サブスクリプションの id によって識別される) 特定のエンドポイントに配信ポリシーを通知を処理します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-169">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="bfacc-170">targetPolicy.platformTypes</span><span class="sxs-lookup"><span data-stu-id="bfacc-170">targetPolicy.platformTypes</span></span> | <span data-ttu-id="bfacc-171">Edm.ComplexType、コレクション (EnumType)</span><span class="sxs-lookup"><span data-stu-id="bfacc-171">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="bfacc-172">フィルター通知の配布を特定のプラットフォームまたはプラットフォームを使用します。</span><span class="sxs-lookup"><span data-stu-id="bfacc-172">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="bfacc-173">既定では、プッシュ エンドポイントのすべての種類 (iOS、ウィンドウ、および Android) が有効になります。</span><span class="sxs-lookup"><span data-stu-id="bfacc-173">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bfacc-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bfacc-174">Relationships</span></span>
<span data-ttu-id="bfacc-175">なし。</span><span class="sxs-lookup"><span data-stu-id="bfacc-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfacc-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfacc-176">JSON representation</span></span>
<span data-ttu-id="bfacc-177">以下は、リソースの JSON 表現は、ターゲット ・ オペレーティング ・ システムに配信する直接視覚的に通知を発行するとき。</span><span class="sxs-lookup"><span data-stu-id="bfacc-177">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

<span data-ttu-id="bfacc-178">次は JSON 表現です、リソースのアプリケーションのクライアントに配信される生データの通知を発行するとき。</span><span class="sxs-lookup"><span data-stu-id="bfacc-178">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
