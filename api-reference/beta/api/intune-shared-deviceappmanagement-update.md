---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0a70c1544ac862b5bbe11f0883d9d2c274a1ad27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920311"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="b9d6b-103">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b9d6b-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="b9d6b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9d6b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9d6b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9d6b-107">[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9d6b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9d6b-108">Prerequisites</span></span>
<span data-ttu-id="b9d6b-109">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b9d6b-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b9d6b-111">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b9d6b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9d6b-112">Permission type</span></span>|<span data-ttu-id="b9d6b-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9d6b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="b9d6b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9d6b-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b9d6b-115">&nbsp;&nbsp; **アプリケーション**、**ブック**、または**契約時**</span><span class="sxs-lookup"><span data-stu-id="b9d6b-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="b9d6b-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9d6b-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b9d6b-117">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="b9d6b-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b9d6b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9d6b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b9d6b-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9d6b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9d6b-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-120">Not supported.</span></span> |
| <span data-ttu-id="b9d6b-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9d6b-121">Application</span></span> | <span data-ttu-id="b9d6b-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9d6b-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9d6b-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="b9d6b-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9d6b-124">Request headers</span></span>
|<span data-ttu-id="b9d6b-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9d6b-125">Header</span></span>|<span data-ttu-id="b9d6b-126">値</span><span class="sxs-lookup"><span data-stu-id="b9d6b-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9d6b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9d6b-127">Authorization</span></span>|<span data-ttu-id="b9d6b-128">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9d6b-129">Accept</span><span class="sxs-lookup"><span data-stu-id="b9d6b-129">Accept</span></span>|<span data-ttu-id="b9d6b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b9d6b-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9d6b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9d6b-131">Request body</span></span>
<span data-ttu-id="b9d6b-132">要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="b9d6b-133">次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="b9d6b-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9d6b-134">Property</span></span>|<span data-ttu-id="b9d6b-135">型</span><span class="sxs-lookup"><span data-stu-id="b9d6b-135">Type</span></span>|<span data-ttu-id="b9d6b-136">説明</span><span class="sxs-lookup"><span data-stu-id="b9d6b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d6b-137">id</span><span class="sxs-lookup"><span data-stu-id="b9d6b-137">id</span></span>|<span data-ttu-id="b9d6b-138">String</span><span class="sxs-lookup"><span data-stu-id="b9d6b-138">String</span></span>|<span data-ttu-id="b9d6b-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-139">Key of the entity.</span></span>|
|<span data-ttu-id="b9d6b-140">**採用**</span><span class="sxs-lookup"><span data-stu-id="b9d6b-140">**On-boarding**</span></span>|
|<span data-ttu-id="b9d6b-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="b9d6b-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="b9d6b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9d6b-142">Boolean</span></span>|<span data-ttu-id="b9d6b-143">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="b9d6b-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="b9d6b-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="b9d6b-145">String</span><span class="sxs-lookup"><span data-stu-id="b9d6b-145">String</span></span>|<span data-ttu-id="b9d6b-146">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="b9d6b-147">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="b9d6b-148">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="b9d6b-149">形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="b9d6b-150">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="b9d6b-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="b9d6b-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="b9d6b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d6b-152">DateTimeOffset</span></span>|<span data-ttu-id="b9d6b-153">ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="b9d6b-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d6b-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b9d6b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d6b-155">DateTimeOffset</span></span>|<span data-ttu-id="b9d6b-156">ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="b9d6b-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="b9d6b-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="b9d6b-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="b9d6b-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="b9d6b-159">エンド ・ ユーザーのポータルの情報は、Intune 企業ポータルにビジネス向けのマイクロソフト ストアからアプリケーションを同期する使用されます。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="b9d6b-160">3 つのオプションから選択するのには\['会社のポータルのみ'、' 企業ポータルおよびプライベート ストアの'、'プライベート ストアのみ'\]。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="b9d6b-161">可能な値は、`none`、`companyPortal`、`privateStore` です。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="b9d6b-162">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="b9d6b-163">応答</span><span class="sxs-lookup"><span data-stu-id="b9d6b-163">Response</span></span>
<span data-ttu-id="b9d6b-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9d6b-165">例</span><span class="sxs-lookup"><span data-stu-id="b9d6b-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9d6b-166">要求</span><span class="sxs-lookup"><span data-stu-id="b9d6b-166">Request</span></span>

<span data-ttu-id="b9d6b-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b9d6b-168">応答</span><span class="sxs-lookup"><span data-stu-id="b9d6b-168">Response</span></span>

<span data-ttu-id="b9d6b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9d6b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



