# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="b3dd5-101">onPremisesConditionalAccessSettings の更新</span><span class="sxs-lookup"><span data-stu-id="b3dd5-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="b3dd5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3dd5-103">[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-103">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3dd5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3dd5-104">Prerequisites</span></span>
<span data-ttu-id="b3dd5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3dd5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3dd5-107">Permission type</span></span>|<span data-ttu-id="b3dd5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3dd5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3dd5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3dd5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b3dd5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3dd5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3dd5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3dd5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3dd5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-112">Not supported.</span></span>|
|<span data-ttu-id="b3dd5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3dd5-113">Application</span></span>|<span data-ttu-id="b3dd5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3dd5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3dd5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="b3dd5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3dd5-116">Request headers</span></span>
|<span data-ttu-id="b3dd5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3dd5-117">Header</span></span>|<span data-ttu-id="b3dd5-118">値</span><span class="sxs-lookup"><span data-stu-id="b3dd5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3dd5-119">承認</span><span class="sxs-lookup"><span data-stu-id="b3dd5-119">Authorization</span></span>|<span data-ttu-id="b3dd5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3dd5-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b3dd5-121">Accept</span></span>|<span data-ttu-id="b3dd5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b3dd5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3dd5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3dd5-123">Request body</span></span>
<span data-ttu-id="b3dd5-124">要求本文で、[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-124">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="b3dd5-125">次の表に、[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-125">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="b3dd5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dd5-126">Property</span></span>|<span data-ttu-id="b3dd5-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="b3dd5-127">Type</span></span>|<span data-ttu-id="b3dd5-128">説明</span><span class="sxs-lookup"><span data-stu-id="b3dd5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3dd5-129">ID</span><span class="sxs-lookup"><span data-stu-id="b3dd5-129">id</span></span>|<span data-ttu-id="b3dd5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dd5-130">String</span></span>|<span data-ttu-id="b3dd5-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3dd5-131">Not yet documented</span></span>|
|<span data-ttu-id="b3dd5-132">有効</span><span class="sxs-lookup"><span data-stu-id="b3dd5-132">enabled</span></span>|<span data-ttu-id="b3dd5-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="b3dd5-133">Boolean</span></span>|<span data-ttu-id="b3dd5-134">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="b3dd5-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="b3dd5-135">includedGroups</span></span>|<span data-ttu-id="b3dd5-136">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dd5-136">Guid collection</span></span>|<span data-ttu-id="b3dd5-137">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="b3dd5-138">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="b3dd5-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="b3dd5-139">excludedGroups</span></span>|<span data-ttu-id="b3dd5-140">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dd5-140">Guid collection</span></span>|<span data-ttu-id="b3dd5-141">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="b3dd5-142">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="b3dd5-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="b3dd5-143">overrideDefaultRule</span></span>|<span data-ttu-id="b3dd5-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="b3dd5-144">Boolean</span></span>|<span data-ttu-id="b3dd5-145">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="b3dd5-146">応答</span><span class="sxs-lookup"><span data-stu-id="b3dd5-146">Response</span></span>
<span data-ttu-id="b3dd5-147">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-147">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3dd5-148">例</span><span class="sxs-lookup"><span data-stu-id="b3dd5-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3dd5-149">要求</span><span class="sxs-lookup"><span data-stu-id="b3dd5-149">Request</span></span>
<span data-ttu-id="b3dd5-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="b3dd5-151">応答</span><span class="sxs-lookup"><span data-stu-id="b3dd5-151">Response</span></span>
<span data-ttu-id="b3dd5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3dd5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "String"
  ],
  "excludedGroups": [
    "String"
  ],
  "overrideDefaultRule": true
}
```








