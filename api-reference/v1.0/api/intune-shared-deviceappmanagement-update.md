---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: c5fc5159af1493fac1e8f280c899914edfd490b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309381"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="6a71b-103">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6a71b-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="6a71b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a71b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a71b-105">[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a71b-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a71b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a71b-106">Prerequisites</span></span>
<span data-ttu-id="6a71b-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="6a71b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6a71b-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a71b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6a71b-109">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6a71b-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6a71b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a71b-110">Permission type</span></span>|<span data-ttu-id="6a71b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a71b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a71b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a71b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a71b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a71b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a71b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a71b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a71b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a71b-115">Not supported.</span></span>|
|<span data-ttu-id="6a71b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a71b-116">Application</span></span>|<span data-ttu-id="6a71b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a71b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a71b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a71b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="6a71b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a71b-119">Request headers</span></span>
|<span data-ttu-id="6a71b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a71b-120">Header</span></span>|<span data-ttu-id="6a71b-121">値</span><span class="sxs-lookup"><span data-stu-id="6a71b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a71b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a71b-122">Authorization</span></span>|<span data-ttu-id="6a71b-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6a71b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a71b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a71b-124">Accept</span></span>|<span data-ttu-id="6a71b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a71b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a71b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a71b-126">Request body</span></span>
<span data-ttu-id="6a71b-127">要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="6a71b-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="6a71b-128">次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a71b-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="6a71b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a71b-129">Property</span></span>|<span data-ttu-id="6a71b-130">種類</span><span class="sxs-lookup"><span data-stu-id="6a71b-130">Type</span></span>|<span data-ttu-id="6a71b-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a71b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a71b-132">ID</span><span class="sxs-lookup"><span data-stu-id="6a71b-132">id</span></span>|<span data-ttu-id="6a71b-133">String</span><span class="sxs-lookup"><span data-stu-id="6a71b-133">String</span></span>|<span data-ttu-id="6a71b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a71b-134">Key of the entity.</span></span>|
|<span data-ttu-id="6a71b-135">**契約時**</span><span class="sxs-lookup"><span data-stu-id="6a71b-135">**Onboarding**</span></span>|
|<span data-ttu-id="6a71b-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="6a71b-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="6a71b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a71b-137">Boolean</span></span>|<span data-ttu-id="6a71b-138">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="6a71b-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="6a71b-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="6a71b-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="6a71b-140">String</span><span class="sxs-lookup"><span data-stu-id="6a71b-140">String</span></span>|<span data-ttu-id="6a71b-141">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="6a71b-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="6a71b-142">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="6a71b-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="6a71b-143">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="6a71b-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="6a71b-144">形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="6a71b-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="6a71b-145">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="6a71b-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="6a71b-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="6a71b-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="6a71b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a71b-147">DateTimeOffset</span></span>|<span data-ttu-id="6a71b-148">ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="6a71b-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="6a71b-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a71b-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="6a71b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a71b-150">DateTimeOffset</span></span>|<span data-ttu-id="6a71b-151">ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="6a71b-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="6a71b-152">応答</span><span class="sxs-lookup"><span data-stu-id="6a71b-152">Response</span></span>
<span data-ttu-id="6a71b-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a71b-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="6a71b-154">要求の例</span><span class="sxs-lookup"><span data-stu-id="6a71b-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="6a71b-155">応答の例</span><span class="sxs-lookup"><span data-stu-id="6a71b-155">Example response</span></span>

<span data-ttu-id="6a71b-156">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="6a71b-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6a71b-157">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a71b-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```


