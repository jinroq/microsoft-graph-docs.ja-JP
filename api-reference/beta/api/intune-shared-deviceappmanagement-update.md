---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6067640d883e771d79e925fd0bcf87c2857c2c0c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967903"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="765a5-103">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="765a5-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="765a5-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="765a5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="765a5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="765a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="765a5-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="765a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="765a5-107">[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="765a5-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="765a5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="765a5-108">Prerequisites</span></span>
<span data-ttu-id="765a5-109">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="765a5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="765a5-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="765a5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="765a5-111">適切なアクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="765a5-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="765a5-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="765a5-112">Permission type</span></span>|<span data-ttu-id="765a5-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="765a5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="765a5-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="765a5-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="765a5-115">&nbsp;&nbsp; **アプリ**、**ブック**、または**オンボード**</span><span class="sxs-lookup"><span data-stu-id="765a5-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="765a5-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="765a5-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="765a5-117">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="765a5-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="765a5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="765a5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="765a5-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="765a5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="765a5-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="765a5-120">Not supported.</span></span> |
| <span data-ttu-id="765a5-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="765a5-121">Application</span></span> | <span data-ttu-id="765a5-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="765a5-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="765a5-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="765a5-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="765a5-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="765a5-124">Request headers</span></span>
|<span data-ttu-id="765a5-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="765a5-125">Header</span></span>|<span data-ttu-id="765a5-126">値</span><span class="sxs-lookup"><span data-stu-id="765a5-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="765a5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="765a5-127">Authorization</span></span>|<span data-ttu-id="765a5-128">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="765a5-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="765a5-129">承諾</span><span class="sxs-lookup"><span data-stu-id="765a5-129">Accept</span></span>|<span data-ttu-id="765a5-130">application/json</span><span class="sxs-lookup"><span data-stu-id="765a5-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="765a5-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="765a5-131">Request body</span></span>
<span data-ttu-id="765a5-132">要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="765a5-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="765a5-133">次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="765a5-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="765a5-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="765a5-134">Property</span></span>|<span data-ttu-id="765a5-135">型</span><span class="sxs-lookup"><span data-stu-id="765a5-135">Type</span></span>|<span data-ttu-id="765a5-136">説明</span><span class="sxs-lookup"><span data-stu-id="765a5-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="765a5-137">id</span><span class="sxs-lookup"><span data-stu-id="765a5-137">id</span></span>|<span data-ttu-id="765a5-138">String</span><span class="sxs-lookup"><span data-stu-id="765a5-138">String</span></span>|<span data-ttu-id="765a5-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="765a5-139">Key of the entity.</span></span>|
|<span data-ttu-id="765a5-140">**オンボード**</span><span class="sxs-lookup"><span data-stu-id="765a5-140">**On-boarding**</span></span>|
|<span data-ttu-id="765a5-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="765a5-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="765a5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="765a5-142">Boolean</span></span>|<span data-ttu-id="765a5-143">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="765a5-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="765a5-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="765a5-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="765a5-145">String</span><span class="sxs-lookup"><span data-stu-id="765a5-145">String</span></span>|<span data-ttu-id="765a5-146">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="765a5-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="765a5-147">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="765a5-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="765a5-148">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="765a5-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="765a5-149">形式は <languagecode2>-<country/regioncode2> です。<languagecode2> は ISO 639-1 に基づく小文字 2 文字で構成されるコードで、<country/regioncode2> は ISO 3166 の基づく大文字 2 文字で構成されるコードです。</span><span class="sxs-lookup"><span data-stu-id="765a5-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="765a5-150">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="765a5-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="765a5-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="765a5-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="765a5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="765a5-152">DateTimeOffset</span></span>|<span data-ttu-id="765a5-153">ビジネス向け Microsoft Store からのアプリケーションの同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="765a5-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="765a5-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="765a5-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="765a5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="765a5-155">DateTimeOffset</span></span>|<span data-ttu-id="765a5-156">Microsoft Store for Business のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="765a5-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="765a5-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="765a5-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="765a5-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="765a5-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="765a5-159">エンドユーザーポータルの情報は、Microsoft Store for Business から Intune ポータルサイトにアプリケーションを同期するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="765a5-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="765a5-160">[会社ポータルのみ]、[ \[ポータルサイトとプライベートストア]、[プライベートストアのみ] から選択するには、3\]つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="765a5-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="765a5-161">使用可能な値は、`none`、`companyPortal`、`privateStore` です。</span><span class="sxs-lookup"><span data-stu-id="765a5-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="765a5-162">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="765a5-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="765a5-163">応答</span><span class="sxs-lookup"><span data-stu-id="765a5-163">Response</span></span>
<span data-ttu-id="765a5-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="765a5-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="765a5-165">例</span><span class="sxs-lookup"><span data-stu-id="765a5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="765a5-166">要求</span><span class="sxs-lookup"><span data-stu-id="765a5-166">Request</span></span>

<span data-ttu-id="765a5-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="765a5-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="765a5-168">応答</span><span class="sxs-lookup"><span data-stu-id="765a5-168">Response</span></span>

<span data-ttu-id="765a5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="765a5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



