# <a name="get-settings"></a><span data-ttu-id="80dcb-101">設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="80dcb-101">Get settings</span></span>

<span data-ttu-id="80dcb-102">ユーザーと組織の[設定](../resources/user_settings.md)オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="80dcb-102">Read the user and organization [settings](../resources/user_settings.md) object.</span></span>
<span data-ttu-id="80dcb-103">[設定](../resources/user_settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定の更新](user_update_settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80dcb-103">To learn how to update the properties of the [settings](../resources/user_settings.md) object, see [update user settings](user_update_settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80dcb-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80dcb-104">Permissions</span></span>

<span data-ttu-id="80dcb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80dcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80dcb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80dcb-107">Permission type</span></span>      | <span data-ttu-id="80dcb-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80dcb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80dcb-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80dcb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="80dcb-110">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80dcb-110">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="80dcb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80dcb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80dcb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80dcb-112">Not supported.</span></span>    |
|<span data-ttu-id="80dcb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80dcb-113">Application</span></span> | <span data-ttu-id="80dcb-114">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80dcb-114">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80dcb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80dcb-115">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="80dcb-116">'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。</span><span class="sxs-lookup"><span data-stu-id="80dcb-116">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="80dcb-117">詳細については、[アクセス許可](../../../concepts/permissions_reference.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80dcb-117">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="80dcb-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="80dcb-118">Request body</span></span>

<span data-ttu-id="80dcb-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80dcb-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80dcb-120">応答</span><span class="sxs-lookup"><span data-stu-id="80dcb-120">Response</span></span>

<span data-ttu-id="80dcb-121">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[ユーザー設定](../resources/user_settings.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="80dcb-121">If successful, this method returns a `200 OK` response code and [user settings](../resources/user_settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80dcb-122">例</span><span class="sxs-lookup"><span data-stu-id="80dcb-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80dcb-123">要求</span><span class="sxs-lookup"><span data-stu-id="80dcb-123">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="80dcb-124">応答</span><span class="sxs-lookup"><span data-stu-id="80dcb-124">Response</span></span>

<span data-ttu-id="80dcb-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80dcb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

