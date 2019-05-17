---
title: ユーザー通知用に Android アプリをクライアント側のSDKと統合する
description: Android アプリをユーザー通知クライアントSDKと統合する
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: 8925dcb7e064015c8ee525e9f1a8c3adc4270f8a
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063363"
---
# <a name="integrate-your-android-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="0f6e1-103">ユーザー通知用に Android アプリをクライアント側のSDKと統合する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-103">Integrate your Android app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="0f6e1-104">Azure ポータルで[アプリを登録](notifications-integration-app-registration.md)し、パートナー デベロッパー センターで[クロスデバイス エクスペリエンス](notifications-integration-cross-device-experiences-onboarding.md)を始めたら、次の手順では、クライアント側の SDK forAndroid とクライアント アプリケーションを統合します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK forAndroid apps.</span></span>  

<span data-ttu-id="0f6e1-105">アプリは、クライアント側の SDK を使い、現在サインインしているユーザーを対象にアプリケーション サーバーから発行された通知の受信を開始するために必要な登録の手順を実行できます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="0f6e1-106">するとSDKは、新しい受信通知の受信、全てを無視するなどのシナリオを実現する通知状態の管理、全ての通知履歴の取得などを含むクライアント側の通知を管理します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="0f6e1-107">新しい受信通知のフロー</span><span class="sxs-lookup"><span data-stu-id="0f6e1-107">New incoming notification flow</span></span>

<span data-ttu-id="0f6e1-108">新しい受信通知を受け取ると、次の図のようなデータ フローが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Android アプリの新しい通知のフロー](images/notifications-new-notification-android.png)

<span data-ttu-id="0f6e1-110">プロセスには、いくつかのコンポーネントが含まれます:</span><span class="sxs-lookup"><span data-stu-id="0f6e1-110">he process involves a few components:</span></span>

* <span data-ttu-id="0f6e1-111">アプリケーション サーバー - アプリケーションのバック エンド</span><span class="sxs-lookup"><span data-stu-id="0f6e1-111">App server - The back end of your application</span></span>
* <span data-ttu-id="0f6e1-112">アプリケーション クライアント - アプリケーションのフロント エンド (UWP アプリ、Android アプリ、または iOS アプリ)</span><span class="sxs-lookup"><span data-stu-id="0f6e1-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="0f6e1-113">Microsoft Graph の通知 - デバイスおよびプラットフォームを跨ぐアプリケーション クライアントの異なるインスタンス間でのユーザー通知の発行と格納、同期を可能にするサービス コンポーネント</span><span class="sxs-lookup"><span data-stu-id="0f6e1-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="0f6e1-114">FCM - Firebase Cloud Messaging のことで、Google Play サービスの一部として Android が提供するプッシュ通知サービス。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-114">FCM - Firebase Cloud Messaging, the push notification service provided by Android as a part of Google Play Services.</span></span> <span data-ttu-id="0f6e1-115">Microsoft Graph の通知は、このサービスを使用して、ユーザーの通知データの変更について Android アプリ クライアントに通知します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-115">Microsoft Graph notifications use this service to signal the Android app clients about user notification data changes.</span></span>  

<span data-ttu-id="0f6e1-116">この図は次の手順を示します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-116">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="0f6e1-117">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-117">Application logic.</span></span> <span data-ttu-id="0f6e1-118">この手順では、ユーザーに発行される通知のトリガーを取り込みます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="0f6e1-119">これは、アプリケーション固有のロジックであり、新しいカレンダー イベントやタスクの割り当て、またはアプリケーション サービス がユーザーに通知したいことなど、Microsoft Graph での他の何かに関するイベントやデータの更新をすることができます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="0f6e1-120">アプリケーション サーバーでは、Microsoft Graph の通知 API 経由で対象のユーザーに通知を発行します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="0f6e1-121">詳細については、[サーバー側との統合](notifications-integrating-app-server.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="0f6e1-122">新しい通知を含む web リクエストを受信すると、Microsoft Graph の通知はこのアプリとユーザー向けに、通知の内容をクラウドで安全に保持します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="0f6e1-123">このユーザーが通知を受け取るための各アプリケーション クライアント インスタンスのサブスクリプションには、Microsoft Graph の通知がオペレーティング システムによって提供されるネイティブ プッシュ サービスを使用して、アプリのクライアントに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="0f6e1-124">この場合、アプリケーションは Android アプリであり、[FCM データメッセージ](https://firebase.google.com/docs/cloud-messaging/concept-options)を使用して信号を送信します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-124">In this case, the application is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
5. <span data-ttu-id="0f6e1-125">受信プッシュ通知によって通知がアプリケーションに送られた後、アプリケーションはユーザー通知ストア内の変更の取得を SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="0f6e1-126">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="0f6e1-127">SDK は、データの変更 (この場合は新しい通知のコンテンツ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="0f6e1-128">変更が正常に取得された後、アプリに通知するためのイベントコールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="0f6e1-129">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-129">Application logic.</span></span> <span data-ttu-id="0f6e1-130">この手順では、使用しているアプリがイベントコールバック内で何を選択しているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="0f6e1-131">通常、ローカルのアプリデータが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="0f6e1-132">この場合、アプリは通常、通知コンテンツをユーザーに通知するトースト通知ポップアップを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-132">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="0f6e1-133">通知の更新フロー</span><span class="sxs-lookup"><span data-stu-id="0f6e1-133">Notification update flow</span></span>

<span data-ttu-id="0f6e1-134">Microsoft Graph の通知を使用するための主な利点の 1 つは、通知が安全にクラウドで保持され、ステートフル リソース タイプ に変更できることです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="0f6e1-135">したがって、アプリケーションはクロスデバイス シナリオにおいて、サインインした同じユーザーに対して、異なるデバイス間で通知の正しい状態を管理して同期することができます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="0f6e1-136">通知が消去としてマークされている場合、または1つのデバイスで既読になっている場合は、その他のデバイスにリアルタイムで通知されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="0f6e1-137">"一度処理すれば、すべての場所で消去される" ということが、ユーザーの通知体験の一部として実現されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="0f6e1-138">次の図は、通知の状態を変更したり、一つのデバイスでの通知を削除したり、別のデバイスで状態の変更または削除を受信/処理するためのデータフローを示しています。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Android アプリの更新通知のフロー](images/notifications-notification-update-android.png)

<span data-ttu-id="0f6e1-140">フローの2番目の部分の通知は、新しい受信通知の処理の流れと似ています。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="0f6e1-141">これは仕様によるものです。SDK のプログラミング パターンは、アプリケーション クライアントがすべての種類のユーザー通知データの変更 (新規着信通知、通知状態の変更、通知の削除) を同様に処理できるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="0f6e1-142">この図は次の手順を示します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-142">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="0f6e1-143">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-143">Application logic.</span></span> <span data-ttu-id="0f6e1-144">何らかのものが、通知を変更または削除するトリガーとなります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="0f6e1-145">通常、あらゆるイベントが通知を変更するトリガーになります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="0f6e1-146">通知を更新または削除するためにクライアント SDK を呼び出すアプリ。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="0f6e1-147">現在、状態の変更に関して2つのプロパティ - **userActionState**と**readstate** -が公開されていますが、アプリケーションはこれらの状態とそれらを更新する必要があるときを定義できます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="0f6e1-148">たとえば、ユーザーが通知ポップアップを終了したときに、**userActionState**を更新して、表示しないようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="0f6e1-149">ユーザーが通知ポップアップをクリックしてアプリを起動し、対応するアプリのコンテンツを使用しているときに、**userActionState**をアクティブ化し、**readState**を読み取りに更新できます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="0f6e1-150">通知を更新または削除するために対応する API が呼び出された後、SDK は、クラウド内のユーザー通知ストアに送信して、同じサインインユーザーの他のアプリクライアントインスタンスにこの変更をファンアウトします。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="0f6e1-151">クライアントから更新/削除要求を受信すると、Microsoft Graph の通知は通知ストアを更新して、この変更をサブスクライブしている他のアプリ クライアント インスタンスを識別します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="0f6e1-152">各アプリケーションの クライアント サブスクリプションには、Microsoft Graph の通知がオペレーティング システムによって提供されるネイティブ プッシュ サービスを使用して、アプリのクライアントに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="0f6e1-153">この場合、これは Android アプリであり、[FCM データメッセージ](https://firebase.google.com/docs/cloud-messaging/concept-options)を使用して信号を送信します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-153">In this case, this is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
6. <span data-ttu-id="0f6e1-154">受信プッシュ通知によって通知がアプリケーションに送られた後、アプリケーションはユーザー通知ストア内の変更の取得を SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="0f6e1-155">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="0f6e1-156">SDK によってデータが変更されます。この場合では、変更内容は通知状態の更新または通知の削除です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="0f6e1-157">変更が正常に取得された後、アプリに通知するためのイベントコールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="0f6e1-158">アプリケーションのロジックです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-158">Application logic.</span></span> <span data-ttu-id="0f6e1-159">この手順では、使用しているアプリがイベントコールバック内で何を選択しているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="0f6e1-160">通常、ローカルのアプリデータが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="0f6e1-161">この場合、通知の更新があるため、アプリはローカルに UI を更新して状態の変更を反映させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="0f6e1-162">たとえば、通知がアクティブ化されている場合、Android 通知トレイ内の対応する通知メッセージを削除すると、"一度処理すれば、すべての場所で消去" することができます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-162">For example, if a notification is marked as activated, you can remove the corresponding notification message inside Android's notification tray to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="0f6e1-163">Microsoft Graph の通知の詳細については、[Microsoft Graph の通知の概要](notifications-concept-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="0f6e1-164">全てを Microsoft Graph の通知と統合するために必要な手順の詳細については、Microsoft Graph の通知の[統合の概要](notifications-integration-e2e-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="development-environment-and-requirements"></a><span data-ttu-id="0f6e1-165">開発環境と要件</span><span class="sxs-lookup"><span data-stu-id="0f6e1-165">Development and authoring requirements</span></span>

<span data-ttu-id="0f6e1-166">Microsoft Graph の通知を使用するには、Android アプリ開発 IDE と、サポートされているアーキテクチャの 1 つ (**armeabi-v7a**、**arm64-v8a**、**x86**、または **x86_64**) を備えた Android デバイス、またはエミュレーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-166">To use Microsoft Graph notifications, you will need an Android app development IDE and an Android device with one of the supported architectures (**armeabi-v7a**, **arm64-v8a**, **x86**, or **x86_64**) or an emulator.</span></span> <span data-ttu-id="0f6e1-167">システムは Android 4.4.2 以降を実行している必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-167">The system must be running Android 4.4.2 or later.</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="0f6e1-168">プロジェクトに SDK を追加する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-168">Adding the references needed to your project</span></span>

<span data-ttu-id="0f6e1-169">プロジェクトのルートにある *build.gradle* ファイルに、次のリポジトリ参照を挿入します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-169">Insert the following repository references into the *build.gradle* file at the root of your project.</span></span>

```Java
allprojects {
    repositories {
    jcenter()
    maven { url 'https://maven.google.com' }
    maven { url 'https://projectrome.bintray.com/maven/' }
    }
}
```

<span data-ttu-id="0f6e1-170">次に、プロジェクトフォルダーにある _build.gradle_ ファイルに次の依存関係を挿入します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-170">Then, insert the following dependency into the _build.gradle_ file that is in your project folder.</span></span>

```Java
dependencies { 
    ...
    implementation 'com.microsoft.connecteddevices:connecteddevices-sdk:+'
}
```

<span data-ttu-id="0f6e1-171">アプリで ProGuard を使用したい場合は、これらの新しい API の ProGuard ルールを追加してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-171">If you want to use ProGuard in your app, add the ProGuard Rules for these new APIs.</span></span> <span data-ttu-id="0f6e1-172">プロジェクトの *App* フォルダに *proguard-rules.txt* というファイルを作成し、[ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt) の内容を貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-172">Create a file called *proguard-rules.txt* in the *App* folder of your project, and paste in the contents of [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span></span>
<span data-ttu-id="0f6e1-173">プロジェクトの *AndroidManifest.xml* ファイルで、`manifest` 要素内に次の権限を追加します (まだ存在しない場合)。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-173">In your project's *AndroidManifest.xml* file, add the following permissions inside the `manifest` element (if they are not already present).</span></span> <span data-ttu-id="0f6e1-174">これにより、インターネットに接続してデバイス上で Bluetooth 検出を有効にする権限がアプリケーションに与えられます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-174">This gives your app permission to connect to the Internet and to enable Bluetooth discovery on your device.</span></span>
<span data-ttu-id="0f6e1-175">Bluetooth 関連の権限は、Bluetooth 検出を使用する場合にのみ必要であり、接続されているデバイス プラットフォームの他の機能には必要ありません。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-175">Note that the Bluetooth-related permissions are only necessary for using Bluetooth discovery; they are not needed for the other features in the Connected Devices Platform.</span></span> <span data-ttu-id="0f6e1-176">また、`ACCESS_COARSE_LOCATION`は Android SDK 21 以降でのみ必須です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-176">Additionally, `ACCESS_COARSE_LOCATION` is only required on Android SDKs 21 and later.</span></span> <span data-ttu-id="0f6e1-177">Android SDK 23 以降では、実行時に位置アクセスを許可するようにユーザーに要求する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-177">On Android SDKs 23 and later, you must also prompt the user to grant location access at runtime.</span></span>

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```
<span data-ttu-id="0f6e1-178">次に、接続デバイス機能を配置するアクティビティのクラスに移動します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-178">Next, go to the activity classes where you would like the Connected Devices functionality to be located.</span></span> <span data-ttu-id="0f6e1-179">次の名前空間をインポートします。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-179">Import the the following namespaces.</span></span>

```java
import com.microsoft.connecteddevices;
import com.microsoft.connecteddevices.userdata;
import com.microsoft.connecteddevices.userdata.usernotifications;
```

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="0f6e1-180">Connected Device Platforms の初期化</span><span class="sxs-lookup"><span data-stu-id="0f6e1-180">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="0f6e1-181">クライアント側のSDKは、Connected Device Platforms と呼ばれるインフラストラクチャの上に構築されています。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-181">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="0f6e1-182">機能を使用するには、アプリ内でプラットフォームを初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-182">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="0f6e1-183">この初期化手順は、通知シナリオを実行する前に必須であるため、メインクラス **OnCreate** メソッド内で実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-183">The initialization steps should occur in your main class **OnCreate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="0f6e1-184">
  [
  \*\*ConnectedDevicesPlatform**](https://docs.microsoft.com/ja-JP/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) クラスをインスタンス化して、プラットフォームを構築および初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-184">You must construct and initialize the platform by instantiating the [**ConnectedDevicesPlatform**](https://docs.microsoft.com/en-us/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) class.</span></span> <span data-ttu-id="0f6e1-185">これを行う前に、プラットフォームが起動した後、イベントが発生する可能性があるため、イベント ハンドラーを接続してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-185">Before doing that, make sure to hook up event handlers, because after the platform is started, the events might begin to fire.</span></span> 

```java
ConnectedDevicesPlatform platform = new ConnectedDevicesPlatform(context);

platform.getAccountManager().accessTokenRequested().subscribe((accountManager, args) -> onAccessTokenRequested(accountManager, args));
platform.getAccountManager().accessTokenInvalidated().subscribe((accountManager, args) -> onAccessTokenInvalidated(accountManager, args));
platform.getNotificationRegistrationManager().notificationRegistrationStateChanged().subscribe((notificationRegistrationManager, args) -> onNotificationRegistrationStateChanged(notificationRegistrationManager, args));

platform.start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="0f6e1-186">アカウント アクセス トークンの処理</span><span class="sxs-lookup"><span data-stu-id="0f6e1-186">Handling account access token</span></span>

<span data-ttu-id="0f6e1-187">新しい受信通知のコンテンツの取得、通知の状態の更新など、SDK が行うすべての Web の呼び出しは、ユーザーのデータに対する読み取りと書き込みであり、そのため常に有効な アクセス トークン を要求します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-187">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="0f6e1-188">プラットフォームが初期化された後に、ユーザーのアクセストークンが正常に機能するために、SDK は次のイベント - アクセス トークン が要求または無効化されたときに呼び出された - の処理を必要とします。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-188">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="0f6e1-189">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="0f6e1-189">accessTokenRequested</span></span> 

<span data-ttu-id="0f6e1-190">完全に実装するには、[Android サンプルアプリ](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-190">For a full implementation, see the [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenRequested(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args) {
    ConnectedDevicesAccessTokenRequest request = args.getRequest();
    List<String> scopes = request.getScopes();

    // We always need to complete the request, even if a matching account is not found
    if (account == null) {
        request.completeWithErrorMessage("The app could not find a matching ConnectedDevicesAccount to get a token");
        return;
    }

    // Complete the request with a token
    account.getAccessTokenAsync(scopes)
        .thenAcceptAsync((String token) -> {
            request.completeWithAccessToken(token);
        }).exceptionally(throwable -> {
            request.completeWithErrorMessage("The Account could not return a token with those scopes");
            return null;
    });
}
```

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="0f6e1-191">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="0f6e1-191">accessTokenInvalidated</span></span>

<span data-ttu-id="0f6e1-192">完全に実装するには、[Android サンプルアプリ](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-192">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args, List<Account> accounts) {
    Log.i(TAG, "Token invalidated for account: " + args.getAccount().getId());
}

```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="0f6e1-193">プッシュ登録の有効期限を処理する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-193">Handling push registration expiration</span></span> 

<span data-ttu-id="0f6e1-194">Microsoft Graph の通知は、FCM、Androidのネイティブのプッシュ プラットフォームを使用して、ユーザー通知のデータ変更をクライアント アプリケーションに通知します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-194">Microsoft Graph notifications uses FCM, the native push platform on Android, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="0f6e1-195">これは、新しい受信通知がアプリサーバーから発行されている場合、またはクロスデバイス シナリオにおいてサインインした同じユーザーの別のデバイスで通知の状態が更新された場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-195">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="0f6e1-196">したがって、データ通知メッセージが正常に送信されることを許可する有効なFCMトークンが必要です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-196">Therefore, a valid FCM token that allows data notification messages to come through successfully is required.</span></span> <span data-ttu-id="0f6e1-197">次のイベントコールバックでは、FCM プッシュトークンの有効期限を処理します。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-197">The following event callback handles FCM push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="0f6e1-198">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="0f6e1-198">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="0f6e1-199">完全に実装するには、[Android サンプルアプリ](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-199">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="0f6e1-200">ユーザーにサインインする</span><span class="sxs-lookup"><span data-stu-id="0f6e1-200">Signing in your user</span></span>

<span data-ttu-id="0f6e1-201">Microsoft Graph 内の他の多くのリソースタイプと同様に、Microsoft Graph の通知は、ユーザーを中核として一元化されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-201">Microsoft Graph notifications, like many other resource types in Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="0f6e1-202">アプリでサブスクライブし、サインインしたユーザーへの通知を受信できるようにするには、最初に登録プロセスで使用する有効な OAuth トークンを入手する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-202">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="0f6e1-203">OAuth トークンを生成および管理する方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-203">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="0f6e1-204">サンプルアプリは ADAL を使用しました。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-204">The sample app used ADAL.</span></span> 

<span data-ttu-id="0f6e1-205">Microsoft アカウント を使用している場合は、サインイン リクエストに次の許可を含める必要があります:`wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-205">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="0f6e1-206">Azure AD アカウントを使用している場合は、次の対象ユーザーをリクエストする必要があります:`https://cdpcs.access.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-206">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="0f6e1-207">プラットフォームにユーザーアカウントを追加する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-207">Adding the user account to the platform</span></span> 

<span data-ttu-id="0f6e1-208">サインインしたユーザーアカウントを SDK に登録する必要があります。これには、FCM を経由して最初のプッシュ通知を受信するためのアカウントの追加とプッシュ チャネルの登録が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-208">You need to register the signed in user account with the SDK, which involves adding the account and registering a push channel in order to receive the initial push notifications through FCM.</span></span> 

```Java
public AsyncOperation<Boolean> prepareAccountAsync(final Context context) {
    // Accounts can be in 3 different scenarios:
    // 1: cached account in good standing (initialized in the SDK and our token cache).
    // 2: account missing from the SDK but present in our cache: Add and initialize account.
    // 3: account missing from our cache but present in the SDK. Log the account out async

    // Subcomponents (e.g. UserDataFeed) can only be initialized when an account is in both the app cache
    // and the SDK cache.
    // For scenario 1, initialize our subcomponents.
    // For scenario 2, subcomponents will be initialized after InitializeAccountAsync registers the account with the SDK.
    // For scenario 3, InitializeAccountAsync will unregister the account and subcomponents will never be initialized.
    switch (mState) {
        // Scenario 1
        case IN_APP_CACHE_AND_SDK_CACHE:
            mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
            return registerAccountWithSdkAsync();
        // Scenario 2
        case IN_APP_CACHE_ONLY: {
            // Add the this account to the ConnectedDevicesPlatform.AccountManager
            return mPlatform.getAccountManager().addAccountAsync(mAccount).thenComposeAsync((ConnectedDevicesAddAccountResult result) -> {
                // We failed to add the account, so exit with a failure to prepare bool
                if (result.getStatus() != ConnectedDevicesAccountAddedStatus.SUCCESS) {
                    result.getStatus());
                    return AsyncOperation.completedFuture(false);
                }

                // Set the registration state of this account as in both app and sdk cache
                mState = AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE;
                mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
                return registerAccountWithSdkAsync();
            });
        }
        // Scenario 3
        case IN_SDK_CACHE_ONLY:
            // Remove the account from the SDK since the app has no knowledge of it
            mPlatform.getAccountManager().removeAccountAsync(mAccount);
            // This account could not be prepared
            return AsyncOperation.completedFuture(false);
        default:
            // This account could not be prepared
            Log.e(TAG, "Failed to prepare account " + mAccount.getId() + " due to unknown state!");
            return AsyncOperation.completedFuture(false);
    }
}
```

```Java
public AsyncOperation<Boolean> registerAccountWithSdkAsync() {
    if (mState != AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE) {
        AsyncOperation<Boolean> toReturn = new AsyncOperation<>();
        toReturn.completeExceptionally(new IllegalStateException("Cannot register this account due to bad state: " + mAccount.getId()));
        return toReturn;
    }

    // Grab the shared GCM/FCM notification token from this app's BroadcastReceiver
    return RomeNotificationReceiver.getNotificationRegistrationAsync().thenComposeAsync((ConnectedDevicesNotificationRegistration notificationRegistration) -> {
        // Perform the registration using the NotificationRegistration
        return mPlatform.getNotificationRegistrationManager().registerAsync(mAccount, notificationRegistration)
            .thenComposeAsync((result) -> {
                if (result.getStatus() == ConnectedDevicesNotificationRegistrationStatus.SUCCESS) {
                    Log.i(TAG, "Successfully registered account " + mAccount.getId() + " for cloud notifications");
                } else {
                    // It would be a good idea for apps to take a look at the different statuses here and perhaps attempt some sort of remediation.
                    // For example, token request failed could mean that the user needs to sign in again. An app could prompt the user for this action 
                    // and retry the operation afterwards.
                    Log.e(TAG, "Failed to register account " + mAccount.getId() + " for cloud notifications!");
                    return AsyncOperation.completedFuture(false);
                }

                return mUserNotificationsManager.registerForAccountAsync();
            });
    });
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="0f6e1-209">ユーザーの通知を受信するためのサブスクライブ</span><span class="sxs-lookup"><span data-stu-id="0f6e1-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="0f6e1-210">このログイン ユーザーのアプリケーションのため、**UserDataFeed** オブジェクトをインスタンス化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-210">You need to instantiate a **UserDataFeed** object for your application for this logged in user.</span></span> <span data-ttu-id="0f6e1-211">アプリケーションは、[クロスデバイス エクスペリエンスの開始](notifications-integration-cross-device-experiences-onboarding.md)に指定したクロスプラットフォームアプリ ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md).</span></span>

```Java
public UserNotificationsManager(@NonNull Context context, @NonNull ConnectedDevicesAccount account, @NonNull ConnectedDevicesPlatform platform)
{
    Context context = new Context;
    UserDataFeed feed = UserDataFeed.getForAccount(account, platform, Secrets.APP_HOST_NAME);
    UserNotificationChannel channel = new UserNotificationChannel(feed);
    UserNotificationReader reader = channel.createReader();
    reader.dataChanged().subscribe((reader, aVoid) -> readFromCache(reader));
    }
}
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="0f6e1-212">ユーザー通知を受信および管理する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="0f6e1-213">このトピックの前のフロー図では、アプリサーバーからの新しい受信通知や、別のアプリケーションクライアントインスタンスから開始された通知の更新または削除を処理するためのプログラミングパターンを示しています。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="0f6e1-214">これらのデータの変更を処理する手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="0f6e1-215">受信プッシュ通知シグナルの処理</span><span class="sxs-lookup"><span data-stu-id="0f6e1-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="0f6e1-216">全ての種類のユーザー通知データの変更について、プッシュ通知としてアプリクライアントに配信されるシグナルが生成されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="0f6e1-217">Android アプリの場合、信号は FCM プッシュ データ メッセージとして配信されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-217">For Android apps, the signal is delivered as a FCM push data message.</span></span> <span data-ttu-id="0f6e1-218">データ メッセージ シグナルを受信するには、アプリが**TryParse**を呼び出し、実際のデータ変更のためのSDKによる Microsoft Graph の通知サービスからの取得をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-218">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```Java
public void onMessageReceived(RemoteMessage message) {
    Map data = message.getData();
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.tryParse(data);

    if (notification != null) {
        try {
            ConnectedDevicesPlatform platform = ConnectedDevicesManager.getConnectedDevicesManager(getApplicationContext()).getPlatform();

            // NOTE: it may be useful to attach completion to this async in order to know when the notification is done being processed.
            // This would be a good time to stop a background service or otherwise cleanup.
            platform.processNotificationAsync(notification);
        } catch (Exception e) {
            Log.e(TAG, "Failed to process FCM notification" + e.getMessage());
        }
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="0f6e1-219">ユーザー通知のデータ変更の処理</span><span class="sxs-lookup"><span data-stu-id="0f6e1-219">Handling user notification data changes</span></span>

<span data-ttu-id="0f6e1-220">SDK がデータ変更の取得を正常に完了すると、イベントコールバックが起こり、アプリクライアントが通知の作成、更新、または削除を処理することが想定されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-220">After the SDK successfully completes fetching the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```Java
private void readFromCache(final UserNotificationReader reader)
{
    reader.readBatchAsync(Long.MAX_VALUE).thenAccept(notifications -> {
        synchronized (this) {
            for (final UserNotification notification : notifications) {
                if (notification.getStatus() == UserNotificationStatus.ACTIVE) {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));

                    if (notification.getUserActionState() == UserNotificationUserActionState.NO_INTERACTION) {
                        mNewNotifications.add(notification);
                        if (notification.getReadState() != UserNotificationReadState.READ) {
                            clearNotification(mContext.getApplicationContext(), notification.getId());
                            addNotification(mContext.getApplicationContext(), notification.getContent(), notification.getId());
                        }
                    } else {
                        clearNotification(mContext.getApplicationContext(), notification.getId());
                    }

                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    mHistoricalNotifications.add(0, notification);
                } else {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));
                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    clearNotification(mContext.getApplicationContext(), notification.getId());
                }
            }
        }

    });
}
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="0f6e1-221">通知の更新状態</span><span class="sxs-lookup"><span data-stu-id="0f6e1-221">Update state of a notification</span></span>

<span data-ttu-id="0f6e1-222">このアプリクライアントインスタンスから通知状態が変更された場合 (たとえば、このデバイスのトースト通知ポップアップがユーザーによって有効化された場合)、アプリは 同じユーザーが使用する全てのデバイスでこの状態の変更を同期するために、SDK を呼び出して通知の状態を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```Java
notification.setUserActionState(UserNotificationUserActionState.ACTIVATED);
notification.saveAsync().whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully activated the notification");
    }
});

```

### <a name="delete-a-notification"></a><span data-ttu-id="0f6e1-223">通知を削除する</span><span class="sxs-lookup"><span data-stu-id="0f6e1-223">Delete a notification</span></span>

<span data-ttu-id="0f6e1-224">このアプリクライアントインスタンスから通知の削除が行われた場合 (たとえば、この通知に対応するタスクが完了とマークされ、アプリのデータベースから削除された場合)、アプリは同じユーザーが使用する全てのデバイスでこの削除の操作を同期するために、SDK を呼び出して通知を削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="0f6e1-225">通知は、有効期限が切れているか、明示的に削除された場合にのみ、ユーザー通知ストアから削除されます。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="0f6e1-226">**Useractionstate**のセマンティック定義はアプリケーション自体によって定義されているため、**Useractionstate**を消去するよう更新しても、ユーザー通知は削除されません。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Java
channel.deleteUserNotificationAsync(notification.getId()).whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully deleted the notification");
    }
});
```

## <a name="see-also"></a><span data-ttu-id="0f6e1-227">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f6e1-227">See also</span></span>

- <span data-ttu-id="0f6e1-228">SDK の通知機能に関連する API のフルセットの [API リファレンス](https://docs.microsoft.com/ja-JP/windows/project-rome/notifications/api-reference-for-android)です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-228">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-android) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="0f6e1-229">Android アプリの[クライアント側のサンプル](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample)です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) for Android apps.</span></span>
- <span data-ttu-id="0f6e1-230">通知を発行するための[アプリサーバーのサンプル](notifications-integrating-app-server.md)です。</span><span class="sxs-lookup"><span data-stu-id="0f6e1-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
