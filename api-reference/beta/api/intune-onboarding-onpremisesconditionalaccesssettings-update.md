---
title: onPremisesConditionalAccessSettings の更新
description: onPremisesConditionalAccessSettings オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 614625dd6783f279dfea9a55d81200184c005844
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317109"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="7c89b-103">onPremisesConditionalAccessSettings の更新</span><span class="sxs-lookup"><span data-stu-id="7c89b-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="7c89b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c89b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c89b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c89b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c89b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c89b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c89b-107">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7c89b-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c89b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c89b-108">Prerequisites</span></span>
<span data-ttu-id="7c89b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c89b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c89b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c89b-111">Permission type</span></span>|<span data-ttu-id="7c89b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c89b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c89b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c89b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c89b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c89b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c89b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c89b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c89b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c89b-116">Not supported.</span></span>|
|<span data-ttu-id="7c89b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c89b-117">Application</span></span>|<span data-ttu-id="7c89b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c89b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c89b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c89b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="7c89b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c89b-120">Request headers</span></span>
|<span data-ttu-id="7c89b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c89b-121">Header</span></span>|<span data-ttu-id="7c89b-122">値</span><span class="sxs-lookup"><span data-stu-id="7c89b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c89b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c89b-123">Authorization</span></span>|<span data-ttu-id="7c89b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c89b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c89b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c89b-125">Accept</span></span>|<span data-ttu-id="7c89b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c89b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c89b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c89b-127">Request body</span></span>
<span data-ttu-id="7c89b-128">要求本文で、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c89b-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="7c89b-129">次の表に、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c89b-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="7c89b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c89b-130">Property</span></span>|<span data-ttu-id="7c89b-131">種類</span><span class="sxs-lookup"><span data-stu-id="7c89b-131">Type</span></span>|<span data-ttu-id="7c89b-132">説明</span><span class="sxs-lookup"><span data-stu-id="7c89b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c89b-133">ID</span><span class="sxs-lookup"><span data-stu-id="7c89b-133">id</span></span>|<span data-ttu-id="7c89b-134">String</span><span class="sxs-lookup"><span data-stu-id="7c89b-134">String</span></span>|<span data-ttu-id="7c89b-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7c89b-135">Not yet documented</span></span>|
|<span data-ttu-id="7c89b-136">enabled</span><span class="sxs-lookup"><span data-stu-id="7c89b-136">enabled</span></span>|<span data-ttu-id="7c89b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c89b-137">Boolean</span></span>|<span data-ttu-id="7c89b-138">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c89b-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="7c89b-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="7c89b-139">includedGroups</span></span>|<span data-ttu-id="7c89b-140">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="7c89b-140">Guid collection</span></span>|<span data-ttu-id="7c89b-141">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="7c89b-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="7c89b-142">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c89b-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="7c89b-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="7c89b-143">excludedGroups</span></span>|<span data-ttu-id="7c89b-144">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="7c89b-144">Guid collection</span></span>|<span data-ttu-id="7c89b-145">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="7c89b-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="7c89b-146">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="7c89b-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="7c89b-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="7c89b-147">overrideDefaultRule</span></span>|<span data-ttu-id="7c89b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c89b-148">Boolean</span></span>|<span data-ttu-id="7c89b-149">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="7c89b-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="7c89b-150">応答</span><span class="sxs-lookup"><span data-stu-id="7c89b-150">Response</span></span>
<span data-ttu-id="7c89b-151">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7c89b-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c89b-152">例</span><span class="sxs-lookup"><span data-stu-id="7c89b-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c89b-153">要求</span><span class="sxs-lookup"><span data-stu-id="7c89b-153">Request</span></span>
<span data-ttu-id="7c89b-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c89b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 201

{
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="7c89b-155">応答</span><span class="sxs-lookup"><span data-stu-id="7c89b-155">Response</span></span>
<span data-ttu-id="7c89b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c89b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





