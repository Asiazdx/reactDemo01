## ����ջ��
react+redux+immutable+less+scss+ES6/7+webpack+fetch+react-router�������+react-transform���滻+webpack-dev-server+http-proxy-middleware
## ����
git clone https://github.com/Asiazdx/reactDemo01.git
cd reactDemo01
npm install
## ���У�nodejs6.0+��
npm run dev (��������ģʽ)
npm run hot(���滻����ģʽ)
����http://localhost:8080
npm run dist(���������汾���Դ�����л���ѹ������ȡ�������룬����css�ļ�)
**˵��**������Ŀ��Ҫ���react��redux��ԭ���Լ�react+redux֮���������Ϲ����ġ�
���ȣ���react��Ҫ��ʲô��react�Ĺ�����ʵ�ܵ�һ����Ҫ������Ⱦ�Ĺ��ع������еĿ�ܣ�����Angular��һ�����ȫ�Ŀ�ܡ�����angular��������Ҫ���������߸�����ϣ�����react��һ������ֻ����
ui��Ⱦ����Ҫ����һ����Ŀ��������Ҫ������͹��ߵ���ϣ�������redux���������ݡ�react-router����·�ɣ�react�Ѿ�ȫ��ӵ��es6������es6Ҳ�����գ�webpack���㲻������ҲҪ���ã���Ҫ������ܣ���Ҫ������أ�
immutable.jsҲ�����ϣ����е�Ԫ���Եȡ�
## React��ʲô
�ýű�����DOM�����Ĵ��ۺܰ����и����еı�������DOM��JavaScript��������Ϊһ�����죬����֮�����շ��������ӣ�jsÿ�η���DOM����Ҫ;�������ţ������ɡ����ŷѡ�������DOM�Ĵ���Խ�࣬���þͻ�Խ�ߡ���Σ��Ƽ���
�������Ǽ��ٹ��ŵĴ�����Ŭ������ECMAScript���ϡ���Ϊ���ԭ��react������dom���Եÿɹ��ˣ�������������dom���������Ǵ洢������ÿ��״̬�����仯��ʱ��ͻᴴ���µ�����ڵ����ǰ�Ľ��жԱȣ��ñ仯�Ĳ��ֽ�����Ⱦ��
��������û�ж�DOM���л�ȡ�Ͳ�����ֻ��һ����Ⱦ�Ĺ��̣�����react����˵��һ��ui��ܡ�
## React�����
react��һ����������Ե���dom��ͼ��state������ɣ�����������μ������state���������ģ�����״̬������ͼ��״̬����ʱ�����ƺ�������һֱ�Ƴ��MVC����ģʽ�е�����û��Controller�����������û�������ô�������ݱ仯˭������
Ȼ���Ⲣ����react��Ҫ���ĵ����飬��ֻ����ui����Ⱦ����������ܼ������ݶ�̬�ı�dom��ͬ��react����setState���ÿ�����ͼ�ĸ��¡�setState���Զ�����render������������ͼ��������Ⱦ���������ֻ��state���ݵı仯��û�е���setState��������
�������¡��������ӵ�ж������ܵ���ͼģ�飬���С��������һ��������������ҳ�������һ���������϶��ɡ����ĺô����������ظ����ú�ά����
## React��Diff�㷨
react��Diff�㷨���������ط��أ���������µ�ʱ��react�ᴴ��һ���µ�����dom�����һ��֮ǰ�洢��dom�����бȽϣ�����ȽϹ��̾��õ���diff�㷨�����������ʼ�����ò����ġ�react�����һ�ּ��裬��ͬ�Ľڵ�������ƵĽṹ������ͬ�ڵ���в�ͬ�ṹ�������ּ���֮��
�������ıȽϣ��������**��Ӧ�Ľڵ��ǲ�ͬ��**���Ǿ�ֱ��ɾ���ɵĽڵ��Լ����������������ӽڵ�Ȼ���滻���µĽڵ㡣**�������ͬ�Ľڵ�**����ֻ�������Եĸ��ġ�
�����б��diff�㷨���в�ͬ����Ϊ�б�ͨ��������ͬ�Ľṹ���ڶ��б�ڵ����ɾ�������룬�����ʱ��danger�ڵ���������Զ��һ�����Ա�һ�����滻Ҫ�õĶࡣ�����ڴ����б��ʱ����Ҫ����keyֵ������react���ܷ���˭��˭����Ȼ��дkeyֵҲ���ԣ�������ͨ���ᱬ�����棬֪ͨ���Ǽ���keyֵ�����react�����ܡ�
## React�������ô����
����Ĵ��췽��ΪReact.createClass()(����һ����)��reactϵͳ�ڲ������һ����ϵͳ��������������react��������Ⲣ���Ǳ���ģ����ǻ�������es6��class�ഴ���������Ҳ��Facebook�ٷ��Ƽ���д����
```javascript
 class Main extends React.Component{
  constructor(props){
    super(prpos);
    this.state={
     productList:[],//��Ʒ�б�
     params:'',//����Ĳ���
    }
   }
 }
 ```
 ������д��ʵ�ֵĹ���һ������ԭ���ǲ�ͬ�ģ�es6��class����Կ����ǹ��캯��ɫһ���﷨�ǣ����԰����������캯�������ġ�extendsʵ������֮��ļ̳� ���� ����һ����Main �̳�React.Component���е����Ժͷ�����
 ������������ں������Ǵ��������ġ�constructor�ǹ���������ʵ��������ʱ���ã�super�����˸����constructor�����˸����ʵ��������this��Ȼ��������Ĺ��캯�������޸ġ����es5��ԭ�ͼ̳��ǲ�ͬ�ģ�ԭ�ͼ̳�����
 ����һ��ʵ��������this��Ȼ���ټ̳и�����ԭ�ͷ������˽�����Щ֮�����ǿ������ʱ�������ܶࡣ
 ������ʹ�����<Main/>ʱ����ʵ�Ƕ�Main���ʵ������new Main��ֻ����react��������̽����˷�װ�������ǿ���������һ����ǩ��
 ������ֵ��ע�⣺1�����������ֵ�����ĸ�����д
 2����Ϊclass����˹ؼ��֣���ѡ������Ҫ��className�����档
 3�����ģ���ڲ�Ĭ��ʹ���ϸ�ģʽ�����Բ���Ҫ��use staticָ������ģʽ��
## �������������
### ����ڳ�ʼ��ʱ�ᴥ��5�����Ӻ���
* getDefaultProps():����Ĭ�ϵ�props��Ҳ������defaultProps���������Ĭ�����ԡ�
* getInitialState():��ʹ��es6��class�﷨ʱ��û��������Ӻ����ģ�����ֱ����constructor�ж���this.state����ʱ���Է���this.props��
* componentWillMount():�����ʼ��ʱֻ���ã��Ժ�������²����ã�������������һ�Σ���ʱ�����޸�state��
* render():react����Ҫ�Ĳ��裬����dom������diff�㷨������dom�����ڴ˽��С���ʱ�Ͳ��ܸ���state�ˡ�
* componentDidMount():�����Ⱦ֮����ã�����ͨ��this.getDOMNode()��ȡ�Ͳ���dom�ڵ㣬ֻ����һ�Ρ�
### �ڸ���ʱ�ᴥ��5�����Ӻ���
* componentWillReceiveProps(nextProps):�����ʼ��ʱ�����ã���������µ�propsʱ����
* shouldComponentUpdate(nextProps,nextState)
react�����Ż��ǳ���Ҫ��һ������������µ�state����propsʱ���ã����ǿ��������ڴ˶Ա�ǰ������props��state�Ƿ���ͬ�������ͬ�򷵻�false��ֹ���£���Ϊ��ͬ
������״̬һ����������ͬ��dom���������Ͳ���Ҫ�����µ�dom���;ɵ�dom������diff�㷨�Աȣ���ʡ�������ܣ�������dom�ṹ���ӵ�ʱ�򡣲�������this.forceUpdate�������˲��衣
* componentWillUpdate(nextProps,nextState)
�����ʼ��ʱ�����ã�ֻ���������Ҫ����ʱ�ŵ��ã���ʱ�����޸�state
* render() ����˵��
* componentDidUpdate()
�����ʼ��ʱ�����ã����������ɺ���ã���ʱ���Ի�ȡdom�ڵ㡣
### ����һ��ж�ع��Ӻ���
componentWillUnmount()
�����Ҫж��ʱ���ã�һЩ�¼������Ͷ�ʱ����Ҫ�ڴ�ʱ�����
���Ͽ��Կ�����react�ܹ���10�����ں�����render�ظ�һ�Σ�����10���������������������ж�����������������õĺÿ��Կ���Ч�ʺ�������ܡ�
## React-Router·��
Router����React��һ�����������������Ⱦ��ֻ��һ�������ڲ�·�ɹ�������ö��󣬸���ƥ���·�ɵ�ַչ����Ӧ�������Route���·�ɵ�ַ��������а󶨣�
Route����Ƕ�׹��ܣ���ʾ·�ɵ�ַ�İ�����ϵ��������֮���Ƕ�ײ�û��ֱ����ϵ��Route������󶨵��������7�����ԣ�children��history��location��params��route��routeParams��routes��
ÿ�����Զ�����·�ɵ������Ϣ���Ƚϳ��õ���children����·�ɵİ�����ϵΪ���ֵ��������location��������ַ����������ַ�л���ʽ��keyֵ��hashֵ����react-router�ṩLink��ǩ����ֻ�Ƕ�a��ǩ��
��װ��ֵ��ע����ǣ�������ӽ�����ת������Ĭ�ϵķ�ʽ��react-route��ֹ��a��ǩ��Ĭ����Ϊ����pushState����hashֵ��ת�䡣�л�ҳ��Ĺ������ڵ��Link��ǩ���ߺ���ǰ����ťʱ�����ȷ���url��ַ��ת�䣬Router��������ַ�ĸı����Route��path����ƥ�䵽��
Ӧ�����������setState����render����������Ⱦdom��
��ҳ��Ƚ϶�ʱ����Ŀ�ͻ�Խ��Խ��������ڵ�ҳ��Ӧ����˵��������Ⱦ���ٶȾͻ���������ʱ�����Ҫ������أ�ֻ���л���ҳ���ʱ���ȥ���ض�Ӧ��js�ļ���react���webpack���а�����صķ����ܼ򵥡�Route��component��ΪgetComponent�������require.ensure�ķ�ʽ��ȡ������webpack������chunkFilename
```javascript
const chooseProducts=(location,cb)=>{
 require.ensure([],require=>{
  cb(null,require('../Component/chooseProducts').default)
 },'chooseProducts')
}
const helpCenter = (location, cb) => {
    require.ensure([], require => {
        cb(null, require('../Component/helpCenter').default)
    },'helpCenter')
}
const saleRecord = (location, cb) => {
    require.ensure([], require => {
        cb(null, require('../Component/saleRecord').default)
    },'saleRecord')
}
const RouteConfig=(
<Router history={history}>
 <Route path="/" component={Roots}>
    <IndexRoute component={index}/>//��ҳ
    <Route path="helpCenter" getComponent={helpCenter}/>//��������
    <Route path="saleRecord" getComponent={saleRecord}/>//���ۼ�¼
    <Redirect from='*' to='/'/>
 </Route>
</Router>
);
 ```
## ���֮���ͨ��
 react�Ƴ���ǵ��������������϶��½������ݴ��ݣ��������¶��ϻ��߲���һ���������ϵ����֮��
 ��ͨ�žͻ��ø��ӡ����ͨ������ķ����кܶ࣬���ֻ�Ǹ��Ӽ���ϵ���������Խ�һ���ص�������������
 ���ݴ��ݸ��Ӽ����Ӽ�����ֱ�ӵ��ú����Ӷ��͸���ͨ�š�
 ����㼶Ƕ�׵��Ƚ������ʹ��������getChildContext��������Ϣ�������ڲ���Ҫ������һ������´����κ�
 һ���Ӽ�������ͨ��this.contextֱ�ӷ��ʡ�
 �ֵܹ�ϵ���֮���޷�ֱ��ͨ�ţ�����ֻ������ͬһ�����ϼ���Ϊ��תս��������ֵ�����Ǹ߲�������Ϊ���ܹ�
 �����ǽ���ͨ�ţ������������������һ�������������������ű������ݣ�������Ϣ�����ã�����ʵ����redux���������顣
 ���֮�����Ϣ������ͨ��ȫ���¼������ݡ���ͬҳ�����ͨ�������������ݣ��¸�ҳ�������location.param����ȡ����ʵreact����
 �ܼ򵥣��ѵ�������������Ÿ�Ч��ʵ�����֮������ݽ�����
 ## Redux
 ���ȣ�redux�����Ǳ���ģ����������൱���ڶ������֮���ּ���һ������������ǽ����߼����㡢�洢���ݺ�ʵ������������Ƕ��������ͨ�š�������֮��
 �Ľ������࣬�߼������ӣ�ֻ�ǵ����Ľ�����ͼ��Ⱦ����ʱ���ûص���contex����û��Ҫ��redux�����˷�����Ӱ�쿪���ٶȡ����������������ر�Ƶ�����߼��ܸ��ӣ�
 ��redux�����ƾ��ر������ˡ�
 �ȼ�˵һ��redux��react����ô��ϵġ�react-redux�ṩ��connect��Provider�����û��ѣ�����һ���������redux����������һ����store������������ͨ��dispatch����action��
 store����action��type���Ե��ö�Ӧ��reducer������state�����action��reducer��state���д�������һ���µ�state����store��connect������store�����仯������setState�������
 ��ʱ�����propsҲ�͸��ű仯��
 ֵ��ע�����connect��Provider��mapStateToProps��mspDispatchToProps��react-redux�ṩ�ģ�redux�����reactû�а�ëǮ�Ĺ�ϵ����ֻ�����ݴ������ģ�û�к�react�����κ���ϣ���
 react-redux��������ϵ��һ��
 ���������Ǿ������һ��react-redux�Ĺ������̡�
 ### redux
 **redux��Ҫ�����������:store,reducer,action**
 store��һ�����������ĸ���Ҫ�ķ�����
#### 1��dispatch
 ����action�ķַ�����createStore�п�����middleware�м����dispatch���и��죬���統action����dispatch����������reducer����Щʱ�����ǲ�ϣ�����������������ǵȴ��첽�������
 ֮���ٴ��������ʱ��redux-thunk��dispatch���и��죬��ǰֻ�ܴ���һ�����󣬸�����ɺ���Դ���һ����������������������ǿ����ֶ�dispatchһ��action��������������ǿɿصģ���ʵ�����첽��
#### 2��subscribe
����state�ı仯�����������store����dispatchʱ��ע��һ��listener����state�仯����������Ҫ֪��state�Ƿ�仯ʱ���Ե��ã�������һ������������������صĺ�������ע��������let unsubscribe=store.subscribe(()=>{console.log('state�����˱仯')})
#### 3��getState
��ȡstore�е�state����������action����reducer�ı���stateʱ����Ҫ���õ��µ�state������ݣ��Ͼ����ݲ���������Ҫ�ġ�getState��Ҫ�������ط��õ���һ����dispatch�õ�action��store��Ҫ��������ȡstate������ݣ�����������ݴ���reducer������������Զ�ִ�еģ�
������������subscribe������state�����仯�����������ȡ�µ�state���ݣ����������һ��˵�����ǳɹ��ˡ�
#### 4��replaceReducer
�滻reducer���ı�state�޸ĵ��߼���
store����ͨ��createStore()����������������������������combineReducers�ϲ���reducer��state�ĳ�ʼ״̬�Լ��ı��dispatch���м�������������������Ǳ���ġ�store����Ҫ�����ǽ�action��reducer��ϵ�������ı�state��
##### action
action��һ����������type�����Ǳ���ģ�ͬʱ���Դ���һЩ���ݡ�action������actionCreactor���д��졣dispatch�䡢���ǰ�action�����ͳ�ȥ��
##### reducer
reducer��һ��������������һ��state��һ��action������action��type����һ���µ�state������ҵ���߼����Է�Ϊ�ܶ��reducer��Ȼ��ͨ��combineReducer�����Ǻϲ���state�����кܶ����ÿ��state�����Ӧһ��reducer��state��������ֿ����ںϲ�ʱ���塣
�������ӣ�
```javascript
 const reducer=combineReducers({
  a:doSomethingWidthA,
  b:processB,
  c:c
 })
```
##### combineReducers
��ʵ��Ҳ��һ��Reducer������������state��һ��action��Ȼ������state��ַ��͸���Ӧ��reducer���д������е�reducer���յ���ͬ��action���������ǻ����action��type�����жϣ��������type���д���Ȼ�󷵻��µ�stateû��type�ͷ���Ĭ��ֵ��Ȼ����Щ��ɢ��state�ֻ�������һ�𷵻�һ���µ�state����
����������һ���������̣����ȵ���store.dispatch��action��Ϊ�������룬ͬʱ��getState��ȡ��ǰ��״̬��state��ע��subscribe��listener����state�仯���ٵ���combineReducers������ȡ��state��action���롣combineReducers�Ὣ�����state�����£����ǵ���subscribe������state�����仯����getState��ȡ
�µ�state���ݡ�
����������һ����������̣����ȵ���store.dispatch��action��Ϊ�������룬ͬʱ��getState��ȡ��ǰ��״̬��state��ע��subscribe��listener����state�仯���ٵ���combineReducers������ȡ��state��action���롣combineReducers�Ὣ�����˵�state��action��������reducer��reducer�����state��keyֵ��ȡ���Լ�
��Ӧ��state��������action��type�����µ�state������state���ĸ��£����ǵ���subscribe������state�����仯����getState��ȡ�µ�state���ݡ�
redux��state��react��state������ȫû�й�ϵ����������һ����
**���������redux����Ҫ���ܣ���ôreact-redux��������ʲô��**
## React-Redux
���ֻʹ��redux����ô�����������ģ�
component-->dispatch(action)-->reducer-->subscribe-->getState-->component
����react-redux֮�������������ģ�
component-->actionCreator(data)-->reducer-->component
store�������ܣ�dispatch,subscribe,getState������Ҫ�ֶ���д�ˡ�react-redux��������������Щ��ͬʱ���ṩ�������û���Provider��һ�������������store��Ϊprops��Ȼ��ͨ��context���´�������react���κ����������ͨ��context��ȡstore��Ҳ����ζ�����ǿ������κ�һ�����������dispatch(action)������redux�ı�state��
����subscribe����state�ı仯��Ȼ����getState��ȡ�仯֮���ֵ�����ǲ����Ƽ������������������������ң����ȵ����Ҳ��Ӱ������ĸ��ã�ά������Ҳ�����鷳��

**connect(mapStateToProps,mapDispatchToProps,mergeProps,option)**��һ���������������ĸ������������ٷ���һ������:**wrapWidthConnrct**,wrapWidthConnect����һ�������Ϊ����wrapWidthConnect(component),���ڲ�����һ�������Connect�������������������������ΪConnect����������return��ȥ��
����������д���������ģ�connect(mapStateToProps,mapDispatchToProps,mergeProps,options)(component)
##### mapStateToProps(state,[ownProps]):
mapStateToProps��������������store��state���Զ����props��������һ���¶�������¶������Ϊprops��һ���ִ���ui��������ǿ��Ը����������Ҫ�������Զ��巵��һ������ownProps�ı仯Ҳ�ᴥ��mapStateToProps
```javascript
 function mapStateToProps(state){
  return {todos:state.todos};
 }
 ```
##### mapDispatchToProps(dispatch,[ownProps]);
mapDispatchToProps����Ƕ�����ô�غ�store����Ϊprops��һ���ִ���ui���������Ǹ�����������������������bindActionCreators�Ὣaction��dispatch�󶨲�����һ�������������غ�ownPropsһ����Ϊprops��һ���ִ���ui��������Բ���mapDispatchToProps�Ƕ����Ǻ����������ն��᷵��һ����������Ǻ�������������keyֵ��
�����Զ���ġ�
```javascript
 function mapDispatchToProps(dispatch){
  return{
   todoActions:bindActionCreators(todoActionCreators,dispatch),
   counterActions:bindActionors(counterActionCreators,dispatch)
  };
 }
```
mapDispatchToProps���صĶ�����������ʵ����һ����actionCreator����Ϊ�Ѿ���dispatch�󶨣����Ե�����actionCreatorʱ����������action���������ֶ�dispatch��ownProps�ı仯Ҳ�ᴥ��mapDispatchToProps��
##### mergeProps(stateProps,dispatchProps,ownProps);
 ��mapStateToProps()��mapDispatchToProps()���صĶ������������props�ϲ����µ�props�����������Ĭ�Ϸ���Object.assign({},ownProps,stateProps,dispatchProps)�Ľ����
##### option
 pure=true��ʾConnect�����������shouldComponentUpdate�ж�store��state��ownProps����ǳ�Աȣ��ж��Ƿ����仯���Ż����ܡ�Ϊfalse�򲻽��жԱȡ�
��ʵconnect������û����ʲô���󲿷��߼������������ص�wrapWidthConnect������ʵ�ֵģ���ȷ��˵����wrapWidthConnect�ڶ����Connect�����ʵ�ֵġ�
## ������һ��������react-->redux-->react����
һ��Provider�������redux��store��Ϊprops��Ȼ��ͨ��context���´���
����connect�����ڳ�ʼ����ʱ��ὫmapDispatchToProps����󶨵�store�����mapDispatchToProps�Ǻ�������Connect������store�󣬸��ݴ����store.dispatch��actionͨ��bindActionCreators���а󶨣��ٽ����صĶ���󶨵�store��connect�����᷵��һ��wrapWithConnect������ͬʱwrapWithConnect�ᱻ�����Ҵ���һ��ui�����wrapWithConnect�ڲ�ʹ��class Connect extends Component������һ��Connect����������ui�������Connect���������Ȼ��Connect�����ͨ��context���store����ͨ��store.getState���������state���󣬽�state����mapStateToProps����stateProps����mapDispatchToProps�����mapDispatchToProps�����᷵��һ��dispatchProps����stateProps��dispatchProps�Լ�Connect�����props����ͨ��Object.assign()������mergeProps�ϲ�Ϊprops����ui�����Ȼ����ComponentDidMount�е���store.subscribe��ע����һ���ص�����handleChange����state�ı仯��
������ʱui����Ϳ�����props���ҵ�actionCreator�������ǵ���actionCreatorʱ���Զ�����dispatch����dispatch�л����getState��ȡ����state��ͬʱע��һ��listener����state�ı仯��store����õ�state��action����combineReducers��combineReducers�Ὣstate����state��keyֵ�ֱ𴫸���reducer������action����ȫ����reducer��reducer�ᱻ����ִ�н���action.type���жϣ�������򷵻�һ���µ�state�����û���򷵻�Ĭ�ϡ�combineReducers�ٴν���reducer���صĵ���state���кϲ���һ���µ�������state����ʱstate�����˱仯��dispatch��state�����µ�ֵ֮����������ע���listener�������а���handleChange������handleChange�����ڲ����ȵ���getState��ȡ�µ�stateֵ�����¾�����state����ǳ�Աȣ������ֱͬ��return�������ͬ�����mapStateToProps��ȡstateProps�����¾�����stateProps����ǳ�Աȣ������ͬ��ֱ��return�����������к����������������ͬ�����this.setState()����Connect����ĸ��£�����ui���������ui����ĸ��£���ʱui�������µ�props��react --> redux --> react ��һ�����̽�����
## ������е㸴�ӣ��򻯰�������ǣ�
һ��Provider�������redux��store��Ϊprops��Ȼ��ͨ��context���´���
����connect�����յ�Provider������store��Ȼ�������������mapStateToProps��mapDispatchToProps�����������state��actionCreator��props�����������ʱ����Ϳ��Ե���actionCreator����������reducer���������µ�state��connect������state�仯����setState������������µ�state���������

connect����д�ķǳ���࣬mapStateToProps��mapDispatchToPropsֻ�����Ǵ���Ļص�������connect�����ڱ�Ҫ��ʱ���������ǣ����ֲ��ǹ̶��ģ��������Բ�д���֡�
�򻯰汾��connect(state => state, action)(Component);
## ��Ŀ�
����˵��react��react-router��redux��֪ʶ�㡣�������������������������һ����������Ŀ��
1��������react.js,redux,react-router�Ȼ����ļ�������npm��װ���������ļ������á�
2����react.js��redux,react-router����������Ҫ�Ķ���ͷ�����
```javscript
 import React, {Component, PropTypes} from 'react';
 import ReactDOM, {render} from 'react-dom';
 import {Provider, connect} from 'react-redux';
 import {createStore, combineReducers, applyMiddleware} from 'redux';
 import { Router, Route, Redirect, IndexRoute, browserHistory, hashHistory } from 'react-router';
 ```
3���������󴴽�����ui�����ÿ������ui�����Ӧһ��ҳ�档
4������actionCreator��reducers������combineReducer�����е�reducer�ϲ���һ�����reducer������createStore����store
������combineReducers��applyMiddleware��
5������connect��actionCreator��reuder�Ͷ����ui������й���������һ���µ������
6������connect���ص��µ�������react-router����·�ɵĲ��𣬷���һ��·�����Router��
7����Router����������Provider������store��ΪProvider�����ԡ�
8������render��ȾProvider����ҷ���ҳ��ı�ǩ�С�
���Կ��������ui�����ʵ�������Ĳ������Provider��Router��Route��Connect�����ĸ��������������ͼ�ϸı�react������ֻ�ǹ����Եġ�
ͨ�������ڶ����ui�����ӡpropsʱ���Կ���һ�����ԣ�
��ͼ�Ķ���ui��������ܹ���18��������ոսӴ�react�����ܶ���Щ������ô���ĸе�������ʵ��Щ������������ط���

����Զ�������1����actionCreator���صĶ���6����reducer���ص�state4����Connect�������0�����Լ�Routerע�������7����


