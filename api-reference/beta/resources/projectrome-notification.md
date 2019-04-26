---
title: 通知リソースの種類
description: '指定したユーザーを対象とするアプリサーバーによって発行される通知を表します。 通知は Microsoft Graph に格納され、ユーザーが所有する異なるデバイスエンドポイントに配布されます。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563353"
---
# <a name="notification-resource-type"></a><span data-ttu-id="ce8b3-104">通知リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce8b3-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8b3-105">指定したユーザーを対象とするアプリサーバーによって発行される通知を表します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="ce8b3-106">通知は Microsoft Graph に格納され、ユーザーが所有する異なるデバイスエンドポイントに配布されます。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="ce8b3-107">通知は、Windows、Android、iOS のプラットフォームを含む、オペレーティングシステムによって解釈可能な視覚的な通知のペイロードである場合があります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="ce8b3-108">また、アプリクライアントによって配信および処理されるデータペイロードを使用して、各デバイスで対応するユーザーの動作を決定します。通常は、生成された元のデータペイロードのコンテンツに対応するビジュアル通知 UI を示します。マシン.</span><span class="sxs-lookup"><span data-stu-id="ce8b3-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="ce8b3-109">ユーザーが視覚的な通知を処理すると、アプリクライアントはクライアント側のプロジェクトローマ SDK を使用して、通知を非表示としてマークするなど、Microsoft Graph で対応する通知フィードの状態を更新することができます。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="ce8b3-110">その後、その更新は他のすべてのアプリクライアントエンドポイントに配布され、クライアントは、ユーザーが冗長情報を表示できないようにするために、その変更をそれに応じて処理します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="ce8b3-111">アプリクライアントは、 [Project ローマ SDK](https://github.com/Microsoft/project-rome)を介して、通知履歴として、(非表示とマークされた後でも) 有効期限が切れる前に、後で同じ通知リソースにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="ce8b3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce8b3-112">Methods</span></span>
|<span data-ttu-id="ce8b3-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce8b3-113">Method</span></span> | <span data-ttu-id="ce8b3-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce8b3-114">Return Type</span></span> | <span data-ttu-id="ce8b3-115">説明</span><span class="sxs-lookup"><span data-stu-id="ce8b3-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="ce8b3-116">通知の作成</span><span class="sxs-lookup"><span data-stu-id="ce8b3-116">Create notification</span></span>](../api/projectrome-notification-post.md) | [<span data-ttu-id="ce8b3-117">お知らせ</span><span class="sxs-lookup"><span data-stu-id="ce8b3-117">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="ce8b3-118">通知を作成し、送信します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce8b3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8b3-119">Properties</span></span>
|<span data-ttu-id="ce8b3-120">名前</span><span class="sxs-lookup"><span data-stu-id="ce8b3-120">Name</span></span> | <span data-ttu-id="ce8b3-121">型</span><span class="sxs-lookup"><span data-stu-id="ce8b3-121">Type</span></span> | <span data-ttu-id="ce8b3-122">説明</span><span class="sxs-lookup"><span data-stu-id="ce8b3-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="ce8b3-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="ce8b3-123">targetHostName</span></span> | <span data-ttu-id="ce8b3-124">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-124">String</span></span> | <span data-ttu-id="ce8b3-125">指定されたユーザーについて、呼び出し元サービスが通知を投稿するアプリケーションのホスト名を表します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="ce8b3-126">appnotificationid</span><span class="sxs-lookup"><span data-stu-id="ce8b3-126">appNotificationId</span></span> | <span data-ttu-id="ce8b3-127">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-127">String</span></span> | <span data-ttu-id="ce8b3-128">通知のアプリサーバーによって設定された一意の id。個別の通知を識別して対象にします。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="ce8b3-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8b3-129">expirationDateTime</span></span> | <span data-ttu-id="ce8b3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8b3-130">DateTimeOffset</span></span> | <span data-ttu-id="ce8b3-131">ユーザー通知の UTC 有効期限を設定します。時間が経過すると、通知は Microsoft Graph 通知フィードストアから完全に削除され、通知履歴の一部ではなくなります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="ce8b3-132">最大値は30日です。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="ce8b3-133">payload</span><span class="sxs-lookup"><span data-stu-id="ce8b3-133">payload</span></span> | <span data-ttu-id="ce8b3-134">Edm ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ce8b3-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="ce8b3-135">これは、この通知を受信するアプリクライアントによって配信および消費される生または視覚的なユーザー通知のデータの内容です。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="ce8b3-136">ペイロードコンテンツ</span><span class="sxs-lookup"><span data-stu-id="ce8b3-136">payload.rawContent</span></span> | <span data-ttu-id="ce8b3-137">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-137">String</span></span> | <span data-ttu-id="ce8b3-138">この通知を受信するアプリクライアントによって配信および消費される生のユーザー通知の通知の内容。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="ce8b3-139">POST 通知要求に対しては、少なくとも1つの content-type コンテンツとペイロードコンテンツが有効である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="ce8b3-140">ペイロード</span><span class="sxs-lookup"><span data-stu-id="ce8b3-140">payload.visual</span></span> | <span data-ttu-id="ce8b3-141">Edm ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ce8b3-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="ce8b3-142">各モバイルプラットフォームの通知プラットフォームによって使用され、ユーザーに対してレンダリングされる、ビジュアルユーザー通知のビジュアルコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="ce8b3-143">POST 通知要求に対して、少なくとも1つのコンテンツおよび visualcontent が有効である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="ce8b3-144">ペイロード</span><span class="sxs-lookup"><span data-stu-id="ce8b3-144">payload.visual.title</span></span> | <span data-ttu-id="ce8b3-145">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-145">String</span></span> | <span data-ttu-id="ce8b3-146">ビジュアルユーザー通知のタイトル。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-146">The title of a visual user notification.</span></span> <span data-ttu-id="ce8b3-147">title または body のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-147">Must have either title or body.</span></span> |
| <span data-ttu-id="ce8b3-148">ペイロード</span><span class="sxs-lookup"><span data-stu-id="ce8b3-148">payload.visual.body</span></span> | <span data-ttu-id="ce8b3-149">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-149">String</span></span> | <span data-ttu-id="ce8b3-150">ビジュアルユーザー通知の本文。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-150">The body of a visual user notification.</span></span> <span data-ttu-id="ce8b3-151">title または body のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-151">Must have either title or body.</span></span> |
| <span data-ttu-id="ce8b3-152">displaytimetolive</span><span class="sxs-lookup"><span data-stu-id="ce8b3-152">displayTimeToLive</span></span> | <span data-ttu-id="ce8b3-153">しきい値</span><span class="sxs-lookup"><span data-stu-id="ce8b3-153">Int</span></span> | <span data-ttu-id="ce8b3-154">この通知コンテンツを各プラットフォームの通知ビューアーに保持する時間 (秒単位) を設定します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="ce8b3-155">たとえば、windows デバイスに通知が配信されると、このプロパティの値が toastnotification に渡されます。この値によって、トースト通知がユーザーの Windows アクションセンターに保持される期間が決まります。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="ce8b3-156">priority</span><span class="sxs-lookup"><span data-stu-id="ce8b3-156">priority</span></span> | <span data-ttu-id="ce8b3-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="ce8b3-157">EnumType</span></span> | <span data-ttu-id="ce8b3-158">生のユーザー通知の優先度を示します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="ce8b3-159">既定では、視覚通知は高優先度で送信されます。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="ce8b3-160">有効な値は High と Low です。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="ce8b3-161">groupName</span><span class="sxs-lookup"><span data-stu-id="ce8b3-161">groupName</span></span> | <span data-ttu-id="ce8b3-162">String</span><span class="sxs-lookup"><span data-stu-id="ce8b3-162">String</span></span> | <span data-ttu-id="ce8b3-163">この通知が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="ce8b3-164">これは、通知をグループ化するための開発者によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="ce8b3-165">targetpolicy</span><span class="sxs-lookup"><span data-stu-id="ce8b3-165">targetPolicy</span></span> | <span data-ttu-id="ce8b3-166">Edm ComplexType、JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ce8b3-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="ce8b3-167">ターゲットポリシーオブジェクトは、対象とする必要があるエンドポイントの種類 (Windows、iOS、および Android) と、対象とする必要がある特定のエンドポイント (サブスクリプション id で識別される) の2つの異なるレベルで通知配信ポリシーを処理します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="ce8b3-168">targetpolicy の種類</span><span class="sxs-lookup"><span data-stu-id="ce8b3-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="ce8b3-169">Edm ComplexType、コレクション (EnumType)</span><span class="sxs-lookup"><span data-stu-id="ce8b3-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="ce8b3-170">特定のプラットフォームまたはプラットフォームに対して通知配布をフィルター処理するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="ce8b3-171">既定では、すべてのプッシュエンドポイントの種類 (iOS、Windows、および Android) が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce8b3-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce8b3-172">Relationships</span></span>
<span data-ttu-id="ce8b3-173">なし。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce8b3-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce8b3-174">JSON representation</span></span>
<span data-ttu-id="ce8b3-175">次に示すのは、移行先のオペレーティングシステムに配信される直接の視覚的な通知を発行するときのリソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

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

<span data-ttu-id="ce8b3-176">アプリクライアントに配信される生データ通知を発行するときの、リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce8b3-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
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
