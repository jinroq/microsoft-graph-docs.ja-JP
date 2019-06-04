---
title: ユーザー通知用に iOS アプリをクライアント側のSDKと統合する
description: iOS アプリをユーザー通知クライアントSDKと統合する。
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: 1e0f809e5f6acea272268b76e69e0d86cc18bff0
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063362"
---
# <a name="integrate-your-ios-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="d7812-103">ユーザー通知用に iOS アプリをクライアント側のSDKと統合する</span><span class="sxs-lookup"><span data-stu-id="d7812-103">Integrate your iOS app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="d7812-104">Azure ポータルで[アプリを登録](notifications-integration-app-registration.md)し、パートナー デベロッパー センターで[クロスデバイス体験](notifications-integration-cross-device-experiences-onboarding.md)を始めたら、次の手順では、クライアント側の SDK foriOS とクライアント アプリケーションを統合します。</span><span class="sxs-lookup"><span data-stu-id="d7812-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK foriOS apps.</span></span>  

<span data-ttu-id="d7812-105">アプリは、クライアント側の SDK を使い、現在サインインしているユーザーを対象にアプリケーション サーバーから発行された通知の受信を開始するために必要な登録の手順を実行できます。</span><span class="sxs-lookup"><span data-stu-id="d7812-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="d7812-106">するとSDKは、新しい受信通知の受信、全てを無視するなどのシナリオを実現する通知状態の管理、全ての通知履歴の取得などを含むクライアント側の通知を管理します。</span><span class="sxs-lookup"><span data-stu-id="d7812-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="d7812-107">新しい受信通知のフロー</span><span class="sxs-lookup"><span data-stu-id="d7812-107">New incoming notification flow</span></span>

<span data-ttu-id="d7812-108">新しい受信通知を受け取ると、次の図のようなデータ フローが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![iOS アプリの新しい通知のフロー](images/notifications-new-notification-ios.png)

<span data-ttu-id="d7812-110">プロセスには、いくつかのコンポーネントが含まれます:</span><span class="sxs-lookup"><span data-stu-id="d7812-110">The process involves a few components:</span></span>

* <span data-ttu-id="d7812-111">アプリケーション サーバー - アプリケーションのバック エンド</span><span class="sxs-lookup"><span data-stu-id="d7812-111">App server - The back end of your application</span></span>
* <span data-ttu-id="d7812-112">アプリケーション クライアント - アプリケーションのフロント エンド (UWP アプリ、Android アプリまたは iOS アプリ)</span><span class="sxs-lookup"><span data-stu-id="d7812-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="d7812-113">Microsoft Graph notifications - デバイスおよびプラットフォームを跨ぐアプリケーション クライアント の異なるインスタンス間でのユーザー通知の発行と格納、同期を可能にするサービス コンポーネント</span><span class="sxs-lookup"><span data-stu-id="d7812-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="d7812-114">APNs - Apple for ios アプリによって提供される Apple プッシュ通知サービスです。</span><span class="sxs-lookup"><span data-stu-id="d7812-114">APNs - The Apple Push Notification Service provided by Apple for iOS apps.</span></span> <span data-ttu-id="d7812-115">Microsoft Graph notifications は、このサービスを使用して、ユーザーの通知データの変更についてiOS アプリ クライアントに通知します。</span><span class="sxs-lookup"><span data-stu-id="d7812-115">Microsoft Graph notifications use this service to signal the iOS app clients about user notification data changes.</span></span>  

<span data-ttu-id="d7812-116">この図は次の手順を示します。</span><span class="sxs-lookup"><span data-stu-id="d7812-116">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="d7812-117">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="d7812-117">Application logic.</span></span> <span data-ttu-id="d7812-118">この手順では、ユーザーに発行される通知のトリガーを取り込みます。</span><span class="sxs-lookup"><span data-stu-id="d7812-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="d7812-119">これは、アプリケーション固有のロジックであり、新しいカレンダー イベントやタスクの割り当て、またはアプリケーション サービス がユーザーに通知したいことなど、Microsoft Graph での他の何かに関するイベントやデータの更新をすることができます。</span><span class="sxs-lookup"><span data-stu-id="d7812-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="d7812-120">アプリケーション サーバーでは、Microsoft Graph notifications API 経由で対象のユーザーに通知を発行します。</span><span class="sxs-lookup"><span data-stu-id="d7812-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="d7812-121">詳細については、[サーバー側との統合](notifications-integrating-app-server.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="d7812-122">新しい通知を含む web リクエストを受信すると、Microsoft Graph notifications はこのアプリとユーザー向けに、通知の内容をクラウドで安全に保持します。</span><span class="sxs-lookup"><span data-stu-id="d7812-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="d7812-123">このユーザーが通知を受け取るための各アプリケーション クライアント インスタンスのサブスクリプションには、Microsoft Graph notifications がオペレーティング システムによって提供されるネイティブ プッシュ サービスを使用して、アプリのクライアントに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="d7812-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="d7812-124">この例ではアプリケーションはiOS のアプリで、 [APNs バック グラウンド更新の通知] を使用して通知を送ります。</span><span class="sxs-lookup"><span data-stu-id="d7812-124">In this case, the application is an iOS app, and it uses [APNs background update notification] to send the signal.</span></span> 
5. <span data-ttu-id="d7812-125">受信プッシュ通知によって通知がアプリケーションに送られた後、アプリケーションはユーザー通知ストア内の変更の取得を SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="d7812-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="d7812-126">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="d7812-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="d7812-127">SDK は、データの変更 (この場合は新しい通知のコンテンツ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="d7812-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="d7812-128">変更が正常に取得された後、アプリに通知するためのイベントコールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="d7812-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="d7812-129">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="d7812-129">Application logic.</span></span> <span data-ttu-id="d7812-130">この手順では、使用しているアプリがイベントコールバック内で何を選択しているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="d7812-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="d7812-131">通常、ローカルのアプリデータが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="d7812-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="d7812-132">この場合、アプリは通常、通知コンテンツをユーザーに通知する iOS アラートを作成します。</span><span class="sxs-lookup"><span data-stu-id="d7812-132">In this case,  the app usually constructs an iOS alert to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="d7812-133">通知の更新フロー</span><span class="sxs-lookup"><span data-stu-id="d7812-133">Notification update flow</span></span>

<span data-ttu-id="d7812-134">Microsoft Graph notifications を使用するための主な利点の 1 つは、通知が安全にクラウドで保持され、ステートフル リソース タイプ に変更できることです。</span><span class="sxs-lookup"><span data-stu-id="d7812-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="d7812-135">したがって、アプリケーションはクロスデバイス シナリオにおいて、サインインした同じユーザーに対して、異なるデバイス間で通知の正しい状態を管理して同期することができます。</span><span class="sxs-lookup"><span data-stu-id="d7812-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="d7812-136">通知が消去としてマークされている場合、または1つのデバイスで既読になっている場合は、その他のデバイスにリアルタイムで通知されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="d7812-137">"一度処理すれば、すべての場所で消去される" ということが、ユーザーの通知体験の一部として実現されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="d7812-138">次の図は、通知の状態を変更したり、一つのデバイスでの通知を削除したり、別のデバイスで状態の変更または削除を受信/処理するためのデータフローを示しています。</span><span class="sxs-lookup"><span data-stu-id="d7812-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![iOS アプリの更新通知のフロー](images/notifications-notification-update-ios.png)

<span data-ttu-id="d7812-140">フローの2番目の部分の通知は、新しい受信通知の処理の流れと似ています。</span><span class="sxs-lookup"><span data-stu-id="d7812-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="d7812-141">これは仕様によるものです。 SDK のプログラミングパターンは、あらゆる種類のユーザー通知データの変更 (新規に受信した通知、通知状態の変更、通知の削除など)をアプリケーションクライアントが同じような方法で処理できるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="d7812-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="d7812-142">この図は次の手順を示します。</span><span class="sxs-lookup"><span data-stu-id="d7812-142">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="d7812-143">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="d7812-143">Application logic.</span></span> <span data-ttu-id="d7812-144">何らかのものが、通知を変更または削除するトリガーとなります。</span><span class="sxs-lookup"><span data-stu-id="d7812-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="d7812-145">通常、あらゆるイベントが通知を変更するトリガーになります。</span><span class="sxs-lookup"><span data-stu-id="d7812-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="d7812-146">通知を更新または削除するためにクライアント SDK を呼び出すアプリ。</span><span class="sxs-lookup"><span data-stu-id="d7812-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="d7812-147">現在、状態の変更に関して2つのプロパティ - **userActionState**と**readstate** -が公開されていますが、アプリケーションはこれらの状態とそれらを更新する必要があるときを定義できます。</span><span class="sxs-lookup"><span data-stu-id="d7812-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="d7812-148">たとえば、ユーザーが通知ポップアップを終了したときに、**userActionState**を更新して、表示しないようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="d7812-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="d7812-149">ユーザーが通知ポップアップをクリックしてアプリを起動し、対応するアプリのコンテンツを使用しているときに、**userActionState**をアクティブ化し、**readState**を読み取りに更新できます。</span><span class="sxs-lookup"><span data-stu-id="d7812-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="d7812-150">通知を更新または削除するために対応する API が呼び出された後、SDK は、クラウド内のユーザー通知ストアに送信して、同じサインインユーザーの他のアプリクライアントインスタンスにこの変更をファンアウトします。</span><span class="sxs-lookup"><span data-stu-id="d7812-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="d7812-151">クライアントから更新/削除要求を受信すると、Microsoft Graph notifications は通知ストアを更新して、この変更をサブスクライブしている他のアプリ クライアント インスタンスを識別します。</span><span class="sxs-lookup"><span data-stu-id="d7812-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="d7812-152">各アプリケーションの クライアント サブスクリプションには、Microsoft Graph notifications がオペレーティング システムによって提供されるネイティブ プッシュ サービスを使用して、アプリのクライアントに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="d7812-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="d7812-153">この例では、iOS のアプリで、 [APNs バック グラウンド更新の通知](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CreatingtheNotificationPayload.html#//apple_ref/doc/uid/TP40008194-CH10-SW8)を使用して通知を送ります。</span><span class="sxs-lookup"><span data-stu-id="d7812-153">In this case, this is an iOS, and it uses [APNs background update notification](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CreatingtheNotificationPayload.html#//apple_ref/doc/uid/TP40008194-CH10-SW8) to send the signal.</span></span> 
6. <span data-ttu-id="d7812-154">受信プッシュ通知によって通知がアプリケーションに送られた後、アプリケーションはユーザー通知ストア内の変更の取得を SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="d7812-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="d7812-155">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="d7812-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="d7812-156">SDK によってデータが変更されます。この場合では、変更内容は通知状態の更新または通知の削除です。</span><span class="sxs-lookup"><span data-stu-id="d7812-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="d7812-157">変更が正常に取得された後、アプリに通知するためのイベントコールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="d7812-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="d7812-158">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="d7812-158">Application logic.</span></span> <span data-ttu-id="d7812-159">この手順では、使用しているアプリがイベントコールバック内で何を選択しているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="d7812-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="d7812-160">通常、ローカルのアプリデータが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="d7812-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="d7812-161">この場合、通知の更新があるため、アプリはローカルに UI を更新して状態の変更を反映させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="d7812-162">たとえば、通知がアクティブ化されている場合、iOS 通知センター内の対応するアラート UI を削除すると、"一度処理すれば、すべての場所で消去" することができます。</span><span class="sxs-lookup"><span data-stu-id="d7812-162">For example, if a notification is marked as activated, you can remove the corresponding alert UI inside the iOS notification center to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="d7812-163">Microsoft Graph 通知の詳細については、[Microsoft Graph Notifications の概要](notifications-concept-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="d7812-164">全てを Microsoft Graph notifications と統合するために必要な手順の詳細については、Microsoft Graph notifications の[統合の概要](notifications-integration-e2e-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="d7812-165">プロジェクトに SDK を追加する</span><span class="sxs-lookup"><span data-stu-id="d7812-165">Adding the references needed to your project</span></span>

<span data-ttu-id="d7812-166">Connected Devices Platform にiOS アプリを追加する最も簡単な方法は、[CocoaPods](https://cocoapods.org/) 依存管理マネージャーを使用することです。</span><span class="sxs-lookup"><span data-stu-id="d7812-166">The simplest way to add the Connected Devices Platform to your iOS app is by using the [CocoaPods](https://cocoapods.org/) dependency manager.</span></span> <span data-ttu-id="d7812-167">iOS プロジェクトの*Podfile*に移動し、次のエントリを挿入します。</span><span class="sxs-lookup"><span data-stu-id="d7812-167">Go to your iOS project's *Podfile* and insert the following entry:</span></span>

```ObjectiveC
platform :ios, "10.0"
workspace 'iOSSample'

target 'iOSSample' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  # use_frameworks!

    pod 'ProjectRomeSdk'

  # Pods for iOSSample
```

> [!NOTE]
> <span data-ttu-id="d7812-168">CocoaPodを使用するには、プロジェクトで _.xcworkspace_ ファイルを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-168">In order to consume CocoaPod, you must use the _.xcworkspace_ file in your project.</span></span>

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="d7812-169">Connected Device Platforms の初期化</span><span class="sxs-lookup"><span data-stu-id="d7812-169">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="d7812-170">クライアント側のSDKは、Connected Device Platforms と呼ばれるインフラストラクチャの上に構築されています。</span><span class="sxs-lookup"><span data-stu-id="d7812-170">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="d7812-171">機能を使用するには、アプリ内でプラットフォームを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-171">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="d7812-172">この初期化手順は、通知シナリオを実行する前に必須であるため、**AppDelegate** メソッド内で実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-172">The initialization steps should occur in your **AppDelegate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="d7812-173">[**MCDConnectedDevicesPlatform**](https://docs.microsoft.com/ja-JP/windows/project-rome/objectivec-api/connecteddevices/mcdconnecteddevicesplatform) クラスをインスタンス化して、プラットフォームを構築および初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-173">You must construct and initialize the platform by instantiating the [**MCDConnectedDevicesPlatform**](https://docs.microsoft.com/en-us/windows/project-rome/objectivec-api/connecteddevices/mcdconnecteddevicesplatform) class.</span></span> <span data-ttu-id="d7812-174">これを行う前に、プラットフォームが起動した後、イベントが発生する可能性があるため、以下のようにイベントハンドラーを接続してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-174">efore doing that, make sure to hook up event handlers, as shown, because after platform is started, the events might begin to fire.</span></span>  

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
        
[platform.accountManager.accessTokenRequested subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager, MCDConnectedDevicesAccessTokenRequestedEventArgs* _Nonnull args) {
    // implement the callback;
}];
        
[self.platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
    // implement the callback;
}];
        
[self.platform.notificationRegistrationManager.notificationRegistrationStateChanged subscribe:^(MCDConnectedDevicesNotificationRegistrationManager* _Nonnull manager __unused, MCDConnectedDevicesNotificationRegistrationStateChangedEventArgs* _Nonnull args) {
    // implement the callback
}];
        
[platform start];
```

### <a name="handling-account-access-token"></a><span data-ttu-id="d7812-175">アカウント アクセス トークンの処理</span><span class="sxs-lookup"><span data-stu-id="d7812-175">Handling account access token</span></span>

<span data-ttu-id="d7812-176">新しい受信通知のコンテンツの取得、通知の状態の更新など、SDK が行うすべての web の呼び出しは、ユーザーのデータに対する読み取りと書き込みであり、そのため常に有効な アクセス トークン を要求します。</span><span class="sxs-lookup"><span data-stu-id="d7812-176">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="d7812-177">プラットフォームが初期化された後に、ユーザーのアクセストークンが正常に機能するために、SDK は次のイベント - アクセス トークン が要求または無効化されたときに呼び出された - の処理を必要とします。</span><span class="sxs-lookup"><span data-stu-id="d7812-177">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="d7812-178">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="d7812-178">accessTokenRequested</span></span>

<span data-ttu-id="d7812-179">完全に実装するには、 [iOS サンプルアプリ](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-179">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="d7812-180">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="d7812-180">accessTokenInvalidated</span></span>

<span data-ttu-id="d7812-181">完全に実装するには、 [iOS サンプルアプリ](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-181">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

```ObjectiveC
[platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
}];
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="d7812-182">プッシュ登録の有効期限を処理する</span><span class="sxs-lookup"><span data-stu-id="d7812-182">Handling push registration expiration</span></span> 

<span data-ttu-id="d7812-183">Microsoft Graph notifications は、Apn、iOSのネイティブのプッシュ プラットフォームを使用して、ユーザー通知のデータ変更をクライアント アプリケーションに通知します。</span><span class="sxs-lookup"><span data-stu-id="d7812-183">Microsoft Graph notifications use APNs, the native push platform on iOS, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="d7812-184">これは、新しい受信通知がアプリサーバーから発行されている場合、またはクロスデバイス シナリオにおいてサインインした同じユーザーの別のデバイスで通知の状態が更新された場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="d7812-184">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="d7812-185">このような理由から、バックグラウンドでの更新通知を正常に受信するための有効な APNs トークンが必要です。</span><span class="sxs-lookup"><span data-stu-id="d7812-185">For this reason, a valid APNs token that allows background update notifications to come through successfully is required.</span></span> <span data-ttu-id="d7812-186">次のイベントコールバックでは、APNs プッシュトークンの有効期限を処理します。</span><span class="sxs-lookup"><span data-stu-id="d7812-186">The following event callback handles APNs push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="d7812-187">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="d7812-187">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="d7812-188">完全に実装するには、 [iOS サンプルアプリ](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-188">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="d7812-189">ユーザーにサインインする</span><span class="sxs-lookup"><span data-stu-id="d7812-189">Signing in your user</span></span>

<span data-ttu-id="d7812-190">Microsoft Graph 内の他の多くのリソースタイプと同様に、Microsoft Graph notifications は、ユーザーを中核として一元化されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-190">Microsoft Graph notifications, like many other resource types inside Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="d7812-191">アプリでサブスクライブし、サインインしたユーザーへの通知を受信できるようにするには、最初に登録プロセスで使用する有効な OAuth トークンを入手する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-191">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="d7812-192">OAuth トークンを生成および管理する方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="d7812-192">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="d7812-193">サンプルアプリは ADAL を使用します。</span><span class="sxs-lookup"><span data-stu-id="d7812-193">The sample app uses ADAL.</span></span> 

<span data-ttu-id="d7812-194">Microsoft アカウント を使用している場合は、サインイン リクエストに次の許可を含める必要があります:`wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。</span><span class="sxs-lookup"><span data-stu-id="d7812-194">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="d7812-195">Azure AD アカウントを使用している場合は、次の対象ユーザーをリクエストする必要があります:`https://cdpcs.access.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="d7812-195">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="d7812-196">プラットフォームにユーザーアカウントを追加する</span><span class="sxs-lookup"><span data-stu-id="d7812-196">Adding the user account to the platform</span></span> 

<span data-ttu-id="d7812-197">サインインしたユーザーアカウントを SDK に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-197">You need to register the signed in user account with the SDK.</span></span> <span data-ttu-id="d7812-198">これは、アカウントの追加と、 APN を通じて初期通知を受信するプッシュチャネルの登録を伴います。</span><span class="sxs-lookup"><span data-stu-id="d7812-198">This involves adding the account and registering a push channel to receive the initial push notifications through APNs.</span></span> <span data-ttu-id="d7812-199">詳細については、サンプルの[prepareAccountAsync](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m) メソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7812-199">For details, see the [prepareAccountAsync](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m) method in the sample.</span></span>

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
MCDConnectedDevicesAccount* mcdAccount = [MCDConnectedDevicesAccount new];

[platform.accountManager addAccountAsync:mcdAccount callback:adapter]; 
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="d7812-200">ユーザーの通知を受信するためのサブスクライブ</span><span class="sxs-lookup"><span data-stu-id="d7812-200">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="d7812-201">このサインインユーザーのアプリケーションのため、**UserDataFeed** オブジェクトをインスタンス化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-201">You need to instantiate a **UserDataFeed** object for your application for this signed in user.</span></span> <span data-ttu-id="d7812-202">アプリケーションは、[クロスデバイス エクスペリエンスの開始時](notifications-integration-cross-device-experiences-onboarding.md)に指定したクロスプラットフォームアプリ ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-202">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md) process.</span></span>

```ObjectiveC
// Initialize the feed and subscribe for notifications
MCDUserDataFeed* feed = [MCDUserDataFeed getForAccount:account
                        platform:platform
                        activitySourceHost:APP_HOST_NAME];

NSArray<MCDUserDataFeedSyncScope*>* syncScopes = @[ [MCDUserNotificationChannel syncScope] ];
[feed subscribeToSyncScopesAsync:syncScopes
        callback:^(BOOL success __unused, NSError* _Nullable error __unused) {
    // Start syncing down notifications
    [feed startSync];
}];
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="d7812-203">ユーザー通知を受信および管理する</span><span class="sxs-lookup"><span data-stu-id="d7812-203">Receiving and managing user notifications</span></span>

<span data-ttu-id="d7812-204">このトピックの前のフロー図では、アプリサーバーからの新しい受信通知や、別のアプリケーションクライアントインスタンスから開始された通知の更新または削除を処理するためのプログラミングパターンを示しています。</span><span class="sxs-lookup"><span data-stu-id="d7812-204">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="d7812-205">これらのデータの変更を処理する手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d7812-205">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="d7812-206">受信プッシュ通知シグナルの処理</span><span class="sxs-lookup"><span data-stu-id="d7812-206">Handling incoming push notification signal</span></span>

<span data-ttu-id="d7812-207">全ての種類のユーザー通知データの変更について、プッシュ通知としてアプリクライアントに配信されるシグナルが生成されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-207">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="d7812-208">iOS アプリの場合、シグナルは APNs バックグラウンド更新通知として配信されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-208">In the case of an iOS app, the signal is delivered as an APNs background update notification.</span></span> <span data-ttu-id="d7812-209">データ メッセージ シグナルを受信するには、アプリが**TryParse**を呼び出し、実際のデータ変更のためのSDKによる Microsoft Graph notifications サービスからの取得をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="d7812-209">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```ObjectiveC
// App running in background and received a push notification, launched by user tapping the alert view
MCDConnectedDevicesNotification* notification = [MCDConnectedDevicesNotification tryParse:notificationInfo];
if (notification != nil) {
    [_platformManager.platform processNotificationAsync:notification
            completion:^(NSError* error __unused) {
        // NOTE: it may be useful to attach completion to this async in order to know when the
        // notification is done being processed.
        // This would be a good time to stop a background service or otherwise cleanup.
    }];
} else {
    NSLog(@"Remote notification is not for ConnectedDevicesPlatform, skip processing");
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="d7812-210">ユーザー通知のデータ変更の処理</span><span class="sxs-lookup"><span data-stu-id="d7812-210">Handling user notification data changes</span></span>

<span data-ttu-id="d7812-211">SDK がデータ変更を正常に取得すると、イベントコールバックが起こり、アプリクライアントが通知の作成、更新、または削除を処理することが想定されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-211">After the SDK successfully fetches the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```ObjectiveC
[reader readBatchAsyncWithMaxSize:100 completion:^(NSArray<MCDUserNotification *> * _Nullable notifications,
                                                    NSError * _Nullable error) {
    if (error) {
    } else {
        for (MCDUserNotification* notification in self.notifications) {
        // Handle notification change based on change type;
        }
        }
    }
}];
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="d7812-212">通知の更新状態</span><span class="sxs-lookup"><span data-stu-id="d7812-212">Update state of a notification</span></span>

<span data-ttu-id="d7812-213">このアプリクライアントインスタンスから通知状態が変更された場合 (たとえば、このデバイスのトースト通知ポップアップがユーザーによって有効化された場合)、アプリは 同じユーザーが使用する全てのデバイスでこの状態の変更を同期するために、SDK を呼び出して通知の状態を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-213">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```ObjectiveC
- (void)dismissNotification:(MCDUserNotification*)notification {
    if (notification.userActionState == MCDUserNotificationUserActionStateNoInteraction) {
        [self dismissNotificationFromTrayWithId:notification.notificationId];
        notification.userActionState = MCDUserNotificationUserActionStateDismissed;
        [notification saveAsync:^(__unused MCDUserNotificationUpdateResult * _Nullable result, __unused NSError * _Nullable error) {
        // handle result;
         }];
    }
}
```

### <a name="delete-a-notifications"></a><span data-ttu-id="d7812-214">通知を削除する</span><span class="sxs-lookup"><span data-stu-id="d7812-214">Delete a notifications</span></span>

<span data-ttu-id="d7812-215">このアプリクライアントインスタンスから通知の削除が行われた場合 (たとえば、この通知に対応するタスクが完了とマークされ、アプリのデータベースから削除された場合)、アプリは同じユーザーが使用する全てのデバイスでこの削除の操作を同期するために、SDK を呼び出して通知を削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7812-215">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="d7812-216">通知は、有効期限が切れているか、明示的に削除された場合にのみ、ユーザー通知ストアから削除されます。</span><span class="sxs-lookup"><span data-stu-id="d7812-216">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="d7812-217">**Useractionstate**のセマンティック定義はアプリケーション自体によって定義されているため、**Useractionstate**を消去するよう更新しても、ユーザー通知は削除されません。</span><span class="sxs-lookup"><span data-stu-id="d7812-217">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Obj-C
- (void)deleteNotification:(MCDUserNotification*)notification {
    [_channel deleteUserNotificationAsync:notification.notificationId
     completion:^(__unused MCDUserNotificationUpdateResult* _Nullable result, NSError* _Nullable error) {
        // handle result;
     }];
}
```

## <a name="see-also"></a><span data-ttu-id="d7812-218">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7812-218">See also</span></span>

- <span data-ttu-id="d7812-219">SDK の通知機能に関連する API のフルセットの [API リファレンス](https://docs.microsoft.com/ja-JP/windows/project-rome/notifications/api-reference-for-ios/)です。</span><span class="sxs-lookup"><span data-stu-id="d7812-219">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-ios/) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="d7812-220">Android アプリの[クライアント側のサンプル](https://github.com/Microsoft/project-rome/tree/master/iOS/samples/GraphNotifications)です。</span><span class="sxs-lookup"><span data-stu-id="d7812-220">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/iOS/samples/GraphNotifications) for Android apps.</span></span>
- <span data-ttu-id="d7812-221">通知を発行するための[アプリサーバーのサンプル](notifications-integrating-app-server.md)です。</span><span class="sxs-lookup"><span data-stu-id="d7812-221">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
